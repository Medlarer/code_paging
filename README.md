# code_paging
这是一个通用的分页的小组件
介绍：
    这是一个分页的小组件，最大的特点是可以保留搜索条件。确保每次跳转的可以查询带上上一次的搜索条件。
    创建一个类：
    需要的参数（
    current_page，当前页码，
    total_count，总数据条数，
    base_url，当前url，
    params，搜索条件，
    per_page_num，每页显示的数据量，
    max_page_code，显示的页码
） 
   
   每页显示数据条数：
   def start(self):
   def end(self):
   显示页码：
   def page_html(self):
   注意：考虑极限情况
   page_html_list = ['首页','上一页'，'其他页码','下一页','尾页']
   return ''.join(page_html_list)
