## File Descriptors

Linux has limited file descriptors, so if we don't close any opened file descriptors at the end of the program, there are chances that the further file descriptor open function may crash the program or application.