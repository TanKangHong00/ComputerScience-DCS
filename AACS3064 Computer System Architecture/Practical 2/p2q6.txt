.386
.model flat, stdcall
.stack 4096
ExitProcess PROTO, dwExitCode: DWORD

.data
    ; variable defination
    val4 db 2


.code

main PROC
    ; write your assembly code here
start:
    mov al, val4
    mul val4

    jmp start

    INVOKE ExitProcess, 0
main ENDP
END main