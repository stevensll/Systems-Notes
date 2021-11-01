# Systems-Notes

11/1/21

# lseek

When files are read/written, a "bookmark" is moved
`lseek(int fildes, off_t offset, int whence)` is used to reposition this offset

* `fildes` : the file descriptor
* `offset` : amount of bytes to move
* `whence` : how to move the amount of bytes
  * `SEEK_SET` : set the bookmark at offset bytes
  * `SEEK_CUR` : current bookmark + offset bytes
  * `SEEK_END` : end of file + offset bytes


