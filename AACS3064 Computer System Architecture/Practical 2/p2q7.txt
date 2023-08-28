.386
.model flat, stdcall
.stack 4096
ExitProcess PROTO, dwExitCode: DWORD

.data
    ; variable defination
    val1 db 6


.code

main PROC
    ; write your assembly code here
start:
    mov al, val1
    mul val1

    jmp start

    INVOKE ExitProcess, 0
main ENDP
END main