# AlphaKu

1. Manual to operate server-side 
  To run a server, you need to install `gunicorn` and `gevent`.
  When you run with gunicorn, you can add some parameters to imporve server performance.
  For example, we considered using gevent to run this server concurrently, so 
  we ran gunicorn with following command.
  
  `gunicorn -k gevent --worker-connection 1000 --bind 0.0.0.0:5000 run:app`
  
