GetImageSize proc uses ebx esi edi 
	invoke GetModuleHandle,0
	mov esi,eax
	add esi,(IMAGE_DOS_HEADER ptr [esi]).e_lfanew
	assume esi:ptr IMAGE_NT_HEADERS
	mov eax,[esi].OptionalHeader.SizeOfImage
	ret
GetImageSize endp
