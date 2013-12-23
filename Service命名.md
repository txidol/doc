#Service命名规范
原则上每个业务实体对应一个Service类，命名格式：实体类名+Service。例如：SiteService、SiteDicService。
常用Service方法命名：
方法	举例
根据ID获取业务实体	Site getSite(String siteId) {
// 代码
}
根据Xxx获取业务实体	Site getSiteByXxx(String xxx) {
// 代码
}
新增业务实体	void createSite(Site site) {
// 代码
}
更新业务实体	void updateSite(Site site) {
// 代码
}
删除业务实体	void deleteSite(String siteId) {
// 代码
}
获取所有业务实体列表	List<Site> getAllSite(){
// 代码
}
分页查找业务实体	Page<Site> findSite(SearchModel searchModel) {
// 代码
}
启用业务实体	void enableSite(String siteId) {
// 代码
}
禁用业务实体	void disableSite(String siteId) {
// 代码
}
