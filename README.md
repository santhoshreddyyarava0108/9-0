# 9-0
org 100h
mov dx,offset output
mov ah,9
int 21h
mov cx,10
mov al,9
add al,30h
mov dl,al
print:
mov ah,2
int 21h
dec dl
loop print
mov ah,4Ch
int 21h     
output db "Numbers are: $"
