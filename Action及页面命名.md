#Action命名规范
原则上每个业务实体对应一个Action类，命名格式：实体类名+Action。

例如：SiteAction、SiteDicAction。

常用的Action方法命名：

1.	查看业务实体

		@Action(“site-view”)
		public String view() {
			// 代码
		}
		
2.	新增业务实体（跳转到新增页面）

		@Action(“site-add”)
		public String add() {
			// 代码
		}
		
3.	保存业务实体（提交新增表单）

		@Action(“site-save”)
		public String save() {
			// 代码
		}
		
4.	编辑业务实体（跳转到编辑页面）

		@Action(“site-edit”)
		public String edit() {
			// 代码
		}
		
5.	更新业务实体（提交编辑表单）

		@Action(“site-update”)
		public String update() {
			// 代码
		}
		
6.	删除业务实体

		@Action(“site-delete”)
		public String delete() {
			// 代码
		}
		
7.	查看业务实体列表（包括分页显示）
	
		@Action(“site-list”)
		public String list() {
			// 代码
		}
		
8.	启用业务实体

		@Action(“site-enable”)
		public String enable() {
			// 代码
		}
		
9.	禁用业务实体

		@Action(“site-disable”)
		public String disable() {
			// 代码
		}

对于多个单词组成的业务实体名，其@Action注解的将拆分单词用”-”连接起来。
例如对于SiteDic业务实体，其对应的Aciton是SiteDicAction，其方法上的@Action注解为：

1.	查看业务实体

		@Action(“site-dic-view”)
		public String view() {
			// 代码
		}
		
2.	新增业务实体（跳转到新增页面）

		@Action(“site-dic-add”)
		public String add() {
			// 代码
		}
		
3.	保存业务实体（提交新增表单）

		@Action(“site-dic-save”)
		public String save() {
			// 代码
		}
		
4.	编辑业务实体（跳转到编辑页面）

		@Action(“site-dic-edit”)
		public String edit() {
			// 代码
		}
		
5.	更新业务实体（提交编辑表单）

		@Action(“site-dic-update”)
		public String update() {
			// 代码
		}
		
6.	删除业务实体

		@Action(“site-dic-delete”)
		public String delete() {
			// 代码
		}
		
7.	查看业务实体列表（包括分页显示）

		@Action(“site-dic-list”)
		public String list() {
			// 代码
		}
		
8.	启用业务实体

		@Action(“site-dic-enable”)
		public String enable() {
			// 代码
		}
		
9.	禁用业务实体
	
		@Action(“site-dic-disable”)
		public String disable() {
			// 代码
		}

#页面命名
页面命名与Action中的方法上的@Action注解标识一一对应。

例如：

	@Action(“site-dic-view”)：	site-dic-view.ftl
	@Action(“site-dic-add”)：	site-dic-add.ftl
	@Action(“site-dic-edit”)：	site-dic-edit.ftl
	@Action(“site-dic-list”)：	site-dic-list.ftl
