Usage: test.py [options]
       test.py -l [options] [FILE]

Dump data from redis or load data into redis.

If input or output file is specified, dump to standard output and load
from standard input.

Options:
  -h, --help            show this help message and exit
  -H HOST, --host=HOST  connect to HOST (default localhost)
  -p PORT, --port=PORT  connect to PORT (default 6379)
  -s SOCKET, --socket=SOCKET
                        connect to SOCKET
  -w PASSWORD, --password=PASSWORD
                        connect with PASSWORD
  -c, --cluster         server cluster mode enable
  -l, --load            load data into redis (default is to dump data from
                        redis)
  -d DB, --db=DB        dump or load into DATABASE (0-N, default 0)
  -o OUTPUT, --output=OUTPUT
                        write to OUTPUT instead of stdout (dump mode only)
  -y, --pretty          Split output on multiple lines and indent it (dump
                        mode only)
  -e, --empty           delete all keys in destination db prior to loading
                        (load mode only)
  -E ENCODING, --encoding=ENCODING
                        set encoding to use while decoding data from redis
  -B BACKEND, --backend=BACKEND
                        use specified ijson backend, default is pure Python
                        (load mode only)
