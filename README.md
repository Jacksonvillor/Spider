# Spider


URL管理器：管理待抓取和已抓取的URL集合。（防止重复/循环抓取）


网页下载器：

1.需要用户登录才能访问（HTTPCookieProcessor）
2.需要代理才能访问（ProxyHandler）
3.协议使用HTTPS加密访问（HTTPSHandler）
4.URL自动跳转（HTTPRedirectHandler）
print('特殊情境')
cj = http.cookiejar.CookieJar()
opener = request.build_opener(request.HTTPCookieProcessor(cj))
request.install_opener(opener)
response3 = request.urlopen(url)
print(response3.getcode())
print(cj)l
print(response3.read())



网页解析器：
1.正则表达式（模糊匹配    ）
2.html.parser
3.beautiful soup(第三方插件)
4.lxml


beautifulsoup:
html网页字符串——》创建BS对象(同时将对象下载为一个DOM树)——》针对DOM树作出节点的搜索——》访问节点的名称/属性/文字
soup = BeautifulSoup(
'html_doc',
'html.parser',
from_encoding = 'utf8'
)


