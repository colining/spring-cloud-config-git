# config-server
* 简单而言，由于微服务化，导致配置变得非常非常多，因此出现了专门config-server，
* 主要逻辑就是从git repo 上拉去配置文件，server会自动的拉去最新提交的内容
* 添加bus-amqp，在server更新时，即通知全部的其他client，做到config sever单智能