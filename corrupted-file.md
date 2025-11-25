- we have a corrupted file
- every file type has a hex header
    - **JPEG/JFIF**: `FF D8 FF E0`
    - **PNG**: `89 50 4E 47`
    - **PDF**: `25 50 44 46`
- we use the `string` command we find that it is a **JPEG/JFIF**
- we change the hex header
> (printf '\xff\xd8\xff\xe0) > repair.png