# 更新日志·ULog

#### Ulog03：2020-12-31

- ['div.col-9.mx-auto>h4.mb-1', '标记问题并合并请求给贡献者']
- ['button[data-octo-dimensions="action:click_dismiss,actor_id:52663614,user_id:52663614,repository_id:322965470,repository_nwo:technology-me/Github-zh,context:issues,public:true,repo_has_help_wanted_label:true,repo_has_good_first_issue_label:true,shows_go_to_labels:false"', '关闭']
- ['div.col-9.mx-auto>p.mb-1', '现在，GitHub将帮助发现潜在问题的第一次贡献者标记为  *(a.background)*']

------

- ['span[aria-label="Cannot fork because you own this repository and are not a member of any organizations."]', '*(svg)*复刻']

#### Ulog02：2020-12-27

- ['a.link-gray-dark.no-underline>span:odd', '标签']
- ['a.link-gray-dark.no-underline>span:even', '提交']
- ['a.link-gray-dark.no-underline>span:first', '分支']

------

- ['a[data-ga-click="Repository, find file, location:repo overview"]', '转到文件']
- ['summary[role="button"]>span.d-none.d-md-flex.flex-items-center', '添加文件']
- ['get-repo>details[data-action="toggle:get-repo#onDetailsToggle"]>summary.btn.btn-primary', '*(svg)*代码*(span with background)*']

------

- ['div.flex-shrink-0.col-12.col-md-3','<h2 class="mb-3 h4">About</h2>','<h2 class="mb-3 h4">简介</h2>']
- ['.flex-shrink-0.col-12.col-md-3','    Releases','发行版']
- ['.flex-shrink-0.col-12.col-md-3','    Packages','软件包']

#### Ulog01：2020-12-26

- ['span[data-content="Code"]','代码']
- ['span[data-content="Issues"]','问题'']
- ['span[data-content="Pull requests"]','合并请求']
- ['span[data-content="Discussions"]','讨论'']
- ['span[data-content="Actions"]','动作'']
- ['span[data-content="Projects"]','项目']
- ['span[data-content="Wiki"]','维基']
- ['span[data-content="Security"]','安全']
- ['span[data-content="Insights"]','统计'']
- ['span[data-content="Settings"]','设置']

------

- ['span[data-target="notifications-list-subscription-form.watchButtonCopy"]','*(svg)*关注']
- ['span[data-target="notifications-list-subscription-form.unwatchButtonCopy"]','*(svg)*取消关注']
- ['span[aria-label="Cannot fork because you own this repository and are not a member of any organizations."]','*(svg)*分叉']

------

- ['a[href="/pulls"]', '合并<span class="d-inline d-md-none d-lg-inline">请求</span>']
- ['a[href="/issues"]', '问题']
- ['a[href="/marketplace"]', '开源广场']
- ['a[href="/explore"]', '推荐']

------

- **Star**

```javascript
$(document).ready(function() {
	// Star专用
	var star = $('button[aria-label="Unstar this repository"]');
	var star_text = $('button[aria-label="Unstar this repository"]>span');
	if (star_text.html().indexOf("Unstar") != -1){
		star_text.html('取消星标');
	} else {
		star_text.html('星标');
	}
	star.click(function() {
		if (star_text.html() == '取消星标' || star_text == 'Unstar'){
			star_text.html('星标');
		} else {
			star_text.html('取消星标');
		}
	})
})
```