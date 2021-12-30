# PHP tags
php://stdin, php://stdout and php://stderr ¶
php://stdin, php://stdout and php://stderr allow direct access to the corresponding input or output stream of the PHP process. The stream references a duplicate file descriptor, so if you open php://stdin and later close it, you close only your copy of the descriptor-the actual stream referenced by STDIN is unaffected. It is recommended that you simply use the constants STDIN, STDOUT and STDERR instead of manually opening streams using these wrappers.
