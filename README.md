# CycleTable
通过拦截器将代理消息转发到子类内部，子类内部则通过外部代理提供的dataSource来拷贝成3份，来组成一个3倍于普通长度的TableView，并在其滑动时进行处理，形成可以无限循环滚动的效果。
这样，在外部看起来，使用这个TableView和普通TableView没有什么不同，但是多了一个可以循环滚动的“属性”，可设置的属性isCycleTable，方便切换普通模式和循环滚动模式。
