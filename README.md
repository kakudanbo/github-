# github-
githubexp监控，刷漏洞能手
只需要注册一个服务器酱，把服务器酱的键写到1.png标注的位置就可以了
代码中的：
        response1 = request.get（URL =“ https://api.github.com/search/repositories?q=jumpserver&sort=updated&per_page=10",headers=headers1,verify=False）
        response2 = requests.get（URL =“ https://api.github.com/search/repositories?q=cms&ssort=updated&per_page=10",headers=headers1,verify=False）
         response1 = requests.get(url="https://api.github.com/search/repositories?q=红队行动框架&sort=updated&order=desc",headers=headers1,verify=False)
        response2 = requests.get(url="https://api.github.com/search/repositories?q=tp5.0.24&ssort=updated&order=desc",headers=headers1,verify=False)
链接中的?q=   是要爬取推送查询的关键字，比如我要监控cve-2020的exp我就可以讲链接改成response1 = request.get（URL =“ https://api.github.com/search/repositories?q=CVE-2020&sort=updated&per_page=10",headers=headers1,verify=False）
