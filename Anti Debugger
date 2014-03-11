.386
.model flat, stdcall
.code
	DllMain proc hInstance:DWORD, dwReason:DWORD, lpReserved:DWORD
		assume fs:nothing
		mov eax, dword ptr fs:[18h]
		mov eax, dword ptr ds:[eax+30h]
		movzx eax, byte ptr ds:[eax+2h]
		xor eax, dword ptr ss:[ebp+0Ch] ; Param2
		ret
	DllMain endp
	
	Init proc
		xor eax, eax
		inc eax
		ret
	Init endp
end DllMain
