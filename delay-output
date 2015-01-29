import sys
import time

PYTHON_VERSION = sys.version_info[0]

if len(sys.argv) == 1:
    delay = 1

else:
    delay = float(sys.argv[1])

try:
    while True:
        if PYTHON_VERSION == 3:
            s = sys.stdin.buffer.raw.readline()
            if len(s) == 0:
                break
            sys.stdout.buffer.raw.write(s)
        else:
            s = sys.stdin.readline()
            if len(s) == 0:
                break
            sys.stdout.write(s)

        time.sleep(delay)

except EOFError:
    pass

except KeyboardInterrupt:
    pass
