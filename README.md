# nets-tcp-framed-race

This lab will showcase race conditions and threads.

In the previous lab, the server supported multiple clients via the use of `os.fork()`. However `FramedThreadServer.py` uses threds instead.

One problem with your previous lab, which we did not mention before, is what happens two file transfers occur at the same time for the same file. It is likely that the resulting file will be a jumbled mess and unrecognizeable from the original.

Your assignment is to implement a threaded version of your file transfer client server.  Additionally, you must use mutex's to ensure something reasonable occurs if the same file is transfered at the same time.
