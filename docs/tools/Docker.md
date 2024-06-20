# Docker

## 什么是 Docker

下面是官网的介绍：

> Docker is an open platform for developing, shipping, and running applications. Docker enables you to separate your applications from your infrastructure so you can deliver software quickly. With Docker, you can manage your infrastructure in the same ways you manage your applications. By taking advantage of Docker's methodologies for shipping, testing, and deploying code, you can significantly reduce the delay between writing code and running it in production.

更详细的介绍，参考[官方文档](https://docs.docker.com/get-started/overview/)。

## 为什么要学习 Docker

在人工智能中，Docker 能够将诸如深度学习、机器学习的环境配置打包，类似于 [Anaconda](./Anaconda.md)，但更容易移植到其它机器上，非常适合在多个服务器中同时迅速部署深度学习环境。你只需要配置好一份 image，然后上传到服务器中，或者传输给他人，就可以通过这份 image 迅速地部署一个几乎一模一样的环境，从而省去了复杂而麻烦的环境配置过程。尤其是在复现他人论文中结果的时候，如果能有一份对应环境的 image，那么复现成功的概率也会大大增加。因此，于人工智能的学习而言，学习 Docker 也非常重要。

## 怎么学习 Docker

可以先浏览一下[这篇博客](https://zhuanlan.zhihu.com/p/187505981)，大致了解 Docker 的工作原理。在此之后，初学者最好的教程当然是 Docker 的[官方教程](https://docs.docker.com/guides/get-started/)。更重要的是，务必在实践中学习！你可以使用 [play-with-docker](https://github.com/play-with-docker/play-with-docker?tab=readme-ov-file) 这个开源项目，通过该项目提供的免费云端 Alpine linux 来学习 docker 的用法。

