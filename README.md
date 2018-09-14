# websocket_colectLog
python编写 通过websocket实时查看linux服务器日志，支持多人同时在线查看相同、不同日志，支持自由切换日志

bug：
  1、前段html页面采用的textare标签做日志展示，当日志量大时，前段会卡死
    解决办法：
      将textare标签改为div，直接用div显示日志，并且将日志追加方式使用为 "div".append(html)的方式，可以解决此问题
