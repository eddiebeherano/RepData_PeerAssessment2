


<!DOCTYPE html>
<html lang="en" class="">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    
    
    <title>RepData_PeerAssessment2/storm_data.md at master · Xiaodan/RepData_PeerAssessment2</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="Xiaodan/RepData_PeerAssessment2" name="twitter:title" /><meta content="RepData_PeerAssessment2 - Peer Assessment 2 for Reproducible Research" name="twitter:description" /><meta content="https://avatars3.githubusercontent.com/u/1871047?v=3&amp;s=400" name="twitter:image:src" />
      <meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="https://avatars3.githubusercontent.com/u/1871047?v=3&amp;s=400" property="og:image" /><meta content="Xiaodan/RepData_PeerAssessment2" property="og:title" /><meta content="https://github.com/Xiaodan/RepData_PeerAssessment2" property="og:url" /><meta content="RepData_PeerAssessment2 - Peer Assessment 2 for Reproducible Research" property="og:description" />
      <meta name="browser-stats-url" content="/_stats">
    <link rel="assets" href="https://assets-cdn.github.com/">
    <link rel="xhr-socket" href="/_sockets">
    <meta name="pjax-timeout" content="1000">
    <link rel="sudo-modal" href="/sessions/sudo_modal">

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>
      <meta name="google-analytics" content="UA-3769691-2">

    <meta content="collector.githubapp.com" name="octolytics-host" /><meta content="collector-cdn.github.com" name="octolytics-script-host" /><meta content="github" name="octolytics-app-id" /><meta content="5EBD821C:4529:36CD4E:550DED5B" name="octolytics-dimension-request_id" /><meta content="7695662" name="octolytics-actor-id" /><meta content="eddiebeherano" name="octolytics-actor-login" /><meta content="62dd80c443efd5b510a1fe375a59375692489289166ea5618c69ac1483321f79" name="octolytics-actor-hash" />
    
    <meta content="Rails, view, blob#show" name="analytics-event" />

    
    <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">


    <meta content="authenticity_token" name="csrf-param" />
<meta content="gTwB6lkSzWindOv/uv1R6LKZ1Plm/DDH9iCNS1CDf/4NhIWaJXSAhH9EvhZHqwZxgpIlYvDc6KRile1ETb4oZA==" name="csrf-token" />

    <link href="https://assets-cdn.github.com/assets/github-099e0ecc2851c8aca89ef6dafa191df3b0f2a2c8ad34e134c5473ca1ba0a59b2.css" media="all" rel="stylesheet" />
    <link href="https://assets-cdn.github.com/assets/github2-1171344316fc088255ee2a06c271d14240f1a4e06985fe9e897762947872e858.css" media="all" rel="stylesheet" />
    
    


    <meta http-equiv="x-pjax-version" content="c0f32272c66bfb10ed7d46b7c88c6299">

      
  <meta name="description" content="RepData_PeerAssessment2 - Peer Assessment 2 for Reproducible Research">
  <meta name="go-import" content="github.com/Xiaodan/RepData_PeerAssessment2 git https://github.com/Xiaodan/RepData_PeerAssessment2.git">

  <meta content="1871047" name="octolytics-dimension-user_id" /><meta content="Xiaodan" name="octolytics-dimension-user_login" /><meta content="22245245" name="octolytics-dimension-repository_id" /><meta content="Xiaodan/RepData_PeerAssessment2" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="22245245" name="octolytics-dimension-repository_network_root_id" /><meta content="Xiaodan/RepData_PeerAssessment2" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/Xiaodan/RepData_PeerAssessment2/commits/master.atom" rel="alternate" title="Recent Commits to RepData_PeerAssessment2:master" type="application/atom+xml">

  </head>


  <body class="logged_in  env-production windows vis-public page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>
    <div class="wrapper">
      
      
      


        <div class="header header-logged-in true" role="banner">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" data-ga-click="Header, go to dashboard, icon:logo">
  <span class="mega-octicon octicon-mark-github"></span>
</a>


      <div class="site-search repo-scope js-site-search" role="search">
          <form accept-charset="UTF-8" action="/Xiaodan/RepData_PeerAssessment2/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/Xiaodan/RepData_PeerAssessment2/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
  <input type="text"
    class="js-site-search-field is-clearable"
    data-hotkey="s"
    name="q"
    placeholder="Search"
    data-global-scope-placeholder="Search GitHub"
    data-repo-scope-placeholder="Search"
    tabindex="1"
    autocapitalize="off">
  <div class="scope-badge">This repository</div>
</form>
      </div>
      <ul class="header-nav left" role="navigation">
        <li class="header-nav-item explore">
          <a class="header-nav-link" href="/explore" data-ga-click="Header, go to explore, text:explore">Explore</a>
        </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://gist.github.com" data-ga-click="Header, go to gist, text:gist">Gist</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="/blog" data-ga-click="Header, go to blog, text:blog">Blog</a>
          </li>
        <li class="header-nav-item">
          <a class="header-nav-link" href="https://help.github.com" data-ga-click="Header, go to help, text:help">Help</a>
        </li>
      </ul>

    
<ul class="header-nav user-nav right" id="user-links">
  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link name" href="/eddiebeherano" data-ga-click="Header, go to profile, text:username">
      <img alt="@eddiebeherano" class="avatar" data-user="7695662" height="20" src="https://avatars1.githubusercontent.com/u/7695662?v=3&amp;s=40" width="20" />
      <span class="css-truncate">
        <span class="css-truncate-target">eddiebeherano</span>
      </span>
    </a>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link js-menu-target tooltipped tooltipped-s" href="#" aria-label="Create new..." data-ga-click="Header, create new, icon:add">
      <span class="octicon octicon-plus"></span>
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      
<ul class="dropdown-menu">
  <li>
    <a href="/new" data-ga-click="Header, create new repository, icon:repo"><span class="octicon octicon-repo"></span> New repository</a>
  </li>
  <li>
    <a href="/organizations/new" data-ga-click="Header, create new organization, icon:organization"><span class="octicon octicon-organization"></span> New organization</a>
  </li>


    <li class="dropdown-divider"></li>
    <li class="dropdown-header">
      <span title="Xiaodan/RepData_PeerAssessment2">This repository</span>
    </li>
      <li>
        <a href="/Xiaodan/RepData_PeerAssessment2/issues/new" data-ga-click="Header, create new issue, icon:issue"><span class="octicon octicon-issue-opened"></span> New issue</a>
      </li>
</ul>

    </div>
  </li>

  <li class="header-nav-item">
        <a href="/notifications" aria-label="You have no unread notifications" class="header-nav-link notification-indicator tooltipped tooltipped-s" data-ga-click="Header, go to notifications, icon:read" data-hotkey="g n">
        <span class="mail-status all-read"></span>
        <span class="octicon octicon-inbox"></span>
</a>
  </li>

  <li class="header-nav-item">
    <a class="header-nav-link tooltipped tooltipped-s" href="/settings/profile" id="account_settings" aria-label="Settings" data-ga-click="Header, go to settings, icon:settings">
      <span class="octicon octicon-gear"></span>
    </a>
  </li>

  <li class="header-nav-item">
    <form accept-charset="UTF-8" action="/logout" class="logout-form" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="f1wtExf70k/saiksSnuVpm9qMEEVvsyi8izZ833djDZoy45QQZEQ5sDJiGEFcKGLkTo+JXzXE91hjSnpz7/bow==" /></div>
      <button class="header-nav-link sign-out-button tooltipped tooltipped-s" aria-label="Sign out" data-ga-click="Header, sign out, icon:logout">
        <span class="octicon octicon-sign-out"></span>
      </button>
</form>  </li>

</ul>


    
  </div>
</div>

        

        


      <div id="start-of-content" class="accessibility-aid"></div>
          <div class="site" itemscope itemtype="http://schema.org/WebPage">
    <div id="js-flash-container">
      
    </div>
    <div class="pagehead repohead instapaper_ignore readability-menu">
      <div class="container">
        
<ul class="pagehead-actions">

  <li>
      <form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="kxyMsWUrHChkqQ8t+vtY4TSmtC5uZQjp00AhdSGCdELBj9My5LWI25b8PcYfjbGuFuX/v0Gf+SRGJpv5+U4HOQ==" /></div>    <input id="repository_id" name="repository_id" type="hidden" value="22245245" />

      <div class="select-menu js-menu-container js-select-menu">
        <a href="/Xiaodan/RepData_PeerAssessment2/subscription"
          class="btn btn-sm btn-with-count select-menu-button js-menu-target" role="button" tabindex="0" aria-haspopup="true"
          data-ga-click="Repository, click Watch settings, action:blob#show">
          <span class="js-select-button">
            <span class="octicon octicon-eye"></span>
            Watch
          </span>
        </a>
        <a class="social-count js-social-count" href="/Xiaodan/RepData_PeerAssessment2/watchers">
          0
        </a>

        <div class="select-menu-modal-holder">
          <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
            <div class="select-menu-header">
              <span class="select-menu-title">Notifications</span>
              <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
            </div>

            <div class="select-menu-list js-navigation-container" role="menu">

              <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
                <span class="select-menu-item-icon octicon octicon-check"></span>
                <div class="select-menu-item-text">
                  <input checked="checked" id="do_included" name="do" type="radio" value="included" />
                  <span class="select-menu-item-heading">Not watching</span>
                  <span class="description">Be notified when participating or @mentioned.</span>
                  <span class="js-select-button-text hidden-select-button-text">
                    <span class="octicon octicon-eye"></span>
                    Watch
                  </span>
                </div>
              </div>

              <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                <span class="select-menu-item-icon octicon octicon octicon-check"></span>
                <div class="select-menu-item-text">
                  <input id="do_subscribed" name="do" type="radio" value="subscribed" />
                  <span class="select-menu-item-heading">Watching</span>
                  <span class="description">Be notified of all conversations.</span>
                  <span class="js-select-button-text hidden-select-button-text">
                    <span class="octicon octicon-eye"></span>
                    Unwatch
                  </span>
                </div>
              </div>

              <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                <span class="select-menu-item-icon octicon octicon-check"></span>
                <div class="select-menu-item-text">
                  <input id="do_ignore" name="do" type="radio" value="ignore" />
                  <span class="select-menu-item-heading">Ignoring</span>
                  <span class="description">Never be notified.</span>
                  <span class="js-select-button-text hidden-select-button-text">
                    <span class="octicon octicon-mute"></span>
                    Stop ignoring
                  </span>
                </div>
              </div>

            </div>

          </div>
        </div>
      </div>
</form>
  </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">

    <form accept-charset="UTF-8" action="/Xiaodan/RepData_PeerAssessment2/unstar" class="js-toggler-form starred js-unstar-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="H6GLneXE1X/TNjQoHlwHbhVhzYSiI+6yIFUN9X9ELDsIub1wuW6w3Z6usQEwCbYt/nykN/dUTcQEw12pF2maDw==" /></div>
      <button
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Unstar this repository" title="Unstar Xiaodan/RepData_PeerAssessment2"
        data-ga-click="Repository, click unstar button, action:blob#show; text:Unstar">
        <span class="octicon octicon-star"></span>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/Xiaodan/RepData_PeerAssessment2/stargazers">
          2
        </a>
</form>
    <form accept-charset="UTF-8" action="/Xiaodan/RepData_PeerAssessment2/star" class="js-toggler-form unstarred js-star-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="VvKbYfc0nQmHtxrgPp6BvhW+Oe/MV6OkS/Cskzzey2ssFdNF9NtfZGbt9J6MkwRS8IyHLhU+r/ul/IDFvHx0fQ==" /></div>
      <button
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Star this repository" title="Star Xiaodan/RepData_PeerAssessment2"
        data-ga-click="Repository, click star button, action:blob#show; text:Star">
        <span class="octicon octicon-star"></span>
        Star
      </button>
        <a class="social-count js-social-count" href="/Xiaodan/RepData_PeerAssessment2/stargazers">
          2
        </a>
</form>  </div>

  </li>

        <li>
          <form accept-charset="UTF-8" action="/Xiaodan/RepData_PeerAssessment2/fork" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="j2voLyzGTvb/hd1EJm7MOBakg1iWYd0otSLU52qgOW7p6NqHXlviOjbJv6RrK6gXn/00sOSrypHsoct68KUd/g==" /></div>
            <button
                type="submit"
                class="btn btn-sm btn-with-count"
                data-ga-click="Repository, show fork modal, action:blob#show; text:Fork"
                title="Fork your own copy of Xiaodan/RepData_PeerAssessment2 to your account"
                aria-label="Fork your own copy of Xiaodan/RepData_PeerAssessment2 to your account">
              <span class="octicon octicon-repo-forked"></span>
              Fork
            </button>
            <a href="/Xiaodan/RepData_PeerAssessment2/network" class="social-count">18</a>
</form>        </li>

</ul>

        <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public">
          <span class="mega-octicon octicon-repo"></span>
          <span class="author"><a href="/Xiaodan" class="url fn" itemprop="url" rel="author"><span itemprop="title">Xiaodan</span></a></span><!--
       --><span class="path-divider">/</span><!--
       --><strong><a href="/Xiaodan/RepData_PeerAssessment2" class="js-current-repository" data-pjax="#js-repo-pjax-container">RepData_PeerAssessment2</a></strong>

          <span class="page-context-loader">
            <img alt="" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
          </span>

        </h1>
      </div><!-- /.container -->
    </div><!-- /.repohead -->

    <div class="container">
      <div class="repository-with-sidebar repo-container new-discussion-timeline  ">
        <div class="repository-sidebar clearfix">
            
<nav class="sunken-menu repo-nav js-repo-nav js-sidenav-container-pjax js-octicon-loaders"
     role="navigation"
     data-pjax="#js-repo-pjax-container"
     data-issue-count-url="/Xiaodan/RepData_PeerAssessment2/issues/counts">
  <ul class="sunken-menu-group">
    <li class="tooltipped tooltipped-w" aria-label="Code">
      <a href="/Xiaodan/RepData_PeerAssessment2" aria-label="Code" class="selected js-selected-navigation-item sunken-menu-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /Xiaodan/RepData_PeerAssessment2">
        <span class="octicon octicon-code"></span> <span class="full-word">Code</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>    </li>

      <li class="tooltipped tooltipped-w" aria-label="Issues">
        <a href="/Xiaodan/RepData_PeerAssessment2/issues" aria-label="Issues" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /Xiaodan/RepData_PeerAssessment2/issues">
          <span class="octicon octicon-issue-opened"></span> <span class="full-word">Issues</span>
          <span class="js-issue-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>      </li>

    <li class="tooltipped tooltipped-w" aria-label="Pull requests">
      <a href="/Xiaodan/RepData_PeerAssessment2/pulls" aria-label="Pull requests" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g p" data-selected-links="repo_pulls /Xiaodan/RepData_PeerAssessment2/pulls">
          <span class="octicon octicon-git-pull-request"></span> <span class="full-word">Pull requests</span>
          <span class="js-pull-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>    </li>


      <li class="tooltipped tooltipped-w" aria-label="Wiki">
        <a href="/Xiaodan/RepData_PeerAssessment2/wiki" aria-label="Wiki" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g w" data-selected-links="repo_wiki /Xiaodan/RepData_PeerAssessment2/wiki">
          <span class="octicon octicon-book"></span> <span class="full-word">Wiki</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>      </li>
  </ul>
  <div class="sunken-menu-separator"></div>
  <ul class="sunken-menu-group">

    <li class="tooltipped tooltipped-w" aria-label="Pulse">
      <a href="/Xiaodan/RepData_PeerAssessment2/pulse" aria-label="Pulse" class="js-selected-navigation-item sunken-menu-item" data-selected-links="pulse /Xiaodan/RepData_PeerAssessment2/pulse">
        <span class="octicon octicon-pulse"></span> <span class="full-word">Pulse</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>    </li>

    <li class="tooltipped tooltipped-w" aria-label="Graphs">
      <a href="/Xiaodan/RepData_PeerAssessment2/graphs" aria-label="Graphs" class="js-selected-navigation-item sunken-menu-item" data-selected-links="repo_graphs repo_contributors /Xiaodan/RepData_PeerAssessment2/graphs">
        <span class="octicon octicon-graph"></span> <span class="full-word">Graphs</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>    </li>
  </ul>


</nav>

              <div class="only-with-full-nav">
                  
<div class="clone-url open"
  data-protocol-type="http"
  data-url="/users/set_protocol?protocol_selector=http&amp;protocol_type=clone">
  <h3><span class="text-emphasized">HTTPS</span> clone URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="https://github.com/Xiaodan/RepData_PeerAssessment2.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="ssh"
  data-url="/users/set_protocol?protocol_selector=ssh&amp;protocol_type=clone">
  <h3><span class="text-emphasized">SSH</span> clone URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="git@github.com:Xiaodan/RepData_PeerAssessment2.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="subversion"
  data-url="/users/set_protocol?protocol_selector=subversion&amp;protocol_type=clone">
  <h3><span class="text-emphasized">Subversion</span> checkout URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="https://github.com/Xiaodan/RepData_PeerAssessment2" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>



<p class="clone-options">You can clone with
  <a href="#" class="js-clone-selector" data-protocol="http">HTTPS</a>, <a href="#" class="js-clone-selector" data-protocol="ssh">SSH</a>, or <a href="#" class="js-clone-selector" data-protocol="subversion">Subversion</a>.
  <a href="https://help.github.com/articles/which-remote-url-should-i-use" class="help tooltipped tooltipped-n" aria-label="Get help on which URL is right for you.">
    <span class="octicon octicon-question"></span>
  </a>
</p>


  <a href="github-windows://openRepo/https://github.com/Xiaodan/RepData_PeerAssessment2" class="btn btn-sm sidebar-button" title="Save Xiaodan/RepData_PeerAssessment2 to your computer and use it in GitHub Desktop." aria-label="Save Xiaodan/RepData_PeerAssessment2 to your computer and use it in GitHub Desktop.">
    <span class="octicon octicon-device-desktop"></span>
    Clone in Desktop
  </a>

                <a href="/Xiaodan/RepData_PeerAssessment2/archive/master.zip"
                   class="btn btn-sm sidebar-button"
                   aria-label="Download the contents of Xiaodan/RepData_PeerAssessment2 as a zip file"
                   title="Download the contents of Xiaodan/RepData_PeerAssessment2 as a zip file"
                   rel="nofollow">
                  <span class="octicon octicon-cloud-download"></span>
                  Download ZIP
                </a>
              </div>
        </div><!-- /.repository-sidebar -->

        <div id="js-repo-pjax-container" class="repository-content context-loader-container" data-pjax-container>
          

<a href="/Xiaodan/RepData_PeerAssessment2/blob/b2a9b42f8c9eb7dfe51ecb67830b46ca2b8da5dd/storm_data.md" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:88a9877ed7dde02faf0fa6d6a80282ad -->

<div class="file-navigation js-zeroclipboard-container">
  
<div class="select-menu js-menu-container js-select-menu left">
  <span class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    data-master-branch="master"
    data-ref="master"
    title="master"
    role="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <span class="octicon octicon-git-branch"></span>
    <i>branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </span>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <span class="select-menu-title">Switch branches/tags</span>
        <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Filter branches/tags" class="js-select-menu-tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/Xiaodan/RepData_PeerAssessment2/blob/master/storm_data.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <span class="select-menu-item-text css-truncate-target" title="master">
                master
              </span>
            </a>
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

  <div class="btn-group right">
    <a href="/Xiaodan/RepData_PeerAssessment2/find/master"
          class="js-show-file-finder btn btn-sm empty-icon tooltipped tooltipped-s"
          data-pjax
          data-hotkey="t"
          aria-label="Quickly jump between files">
      <span class="octicon octicon-list-unordered"></span>
    </a>
    <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
  </div>

  <div class="breadcrumb js-zeroclipboard-target">
    <span class='repo-root js-repo-root'><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/Xiaodan/RepData_PeerAssessment2" class="" data-branch="master" data-direction="back" data-pjax="true" itemscope="url"><span itemprop="title">RepData_PeerAssessment2</span></a></span></span><span class="separator">/</span><strong class="final-path">storm_data.md</strong>
  </div>
</div>


  <div class="commit file-history-tease">
    <div class="file-history-tease-header">
        <img alt="Sally Zhang" class="avatar" data-user="1871047" height="24" src="https://avatars1.githubusercontent.com/u/1871047?v=3&amp;s=48" width="24" />
        <span class="author"><a href="/Xiaodan" rel="author">Xiaodan</a></span>
        <time datetime="2014-07-25T22:09:24Z" is="relative-time">Jul 25, 2014</time>
        <div class="commit-title">
            <a href="/Xiaodan/RepData_PeerAssessment2/commit/8f364e212ea8ceca2755d8a79d18ccdc6da10b43" class="message" data-pjax="true" title="Included .md file.">Included .md file.</a>
        </div>
    </div>

    <div class="participation">
      <p class="quickstat">
        <a href="#blob_contributors_box" rel="facebox">
          <strong>1</strong>
           contributor
        </a>
      </p>
      
    </div>
    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list">
          <li class="facebox-user-list-item">
            <img alt="Sally Zhang" data-user="1871047" height="24" src="https://avatars1.githubusercontent.com/u/1871047?v=3&amp;s=48" width="24" />
            <a href="/Xiaodan">Xiaodan</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file">
  <div class="file-header">
    <div class="file-actions">

      <div class="btn-group">
        <a href="/Xiaodan/RepData_PeerAssessment2/raw/master/storm_data.md" class="btn btn-sm " id="raw-url">Raw</a>
          <a href="/Xiaodan/RepData_PeerAssessment2/blame/master/storm_data.md" class="btn btn-sm js-update-url-with-hash">Blame</a>
        <a href="/Xiaodan/RepData_PeerAssessment2/commits/master/storm_data.md" class="btn btn-sm " rel="nofollow">History</a>
      </div>

        <a class="octicon-btn tooltipped tooltipped-nw"
           href="github-windows://openRepo/https://github.com/Xiaodan/RepData_PeerAssessment2?branch=master&amp;filepath=storm_data.md"
           aria-label="Open this file in GitHub for Windows">
            <span class="octicon octicon-device-desktop"></span>
        </a>

            <form accept-charset="UTF-8" action="/Xiaodan/RepData_PeerAssessment2/edit/master/storm_data.md" class="inline-form" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="7dvMTnOieNMpNQoyJR8acbeZ8haJBBgH8OL5VY+ZC/BYdGVzMik9OVOXwtFsZPClD/PrMmkUBx7IvuMTxTQwKA==" /></div>
              <button class="octicon-btn tooltipped tooltipped-n" type="submit" aria-label="Clicking this button will fork this project so you can edit the file" data-hotkey="e" data-disable-with>
                <span class="octicon octicon-pencil"></span>
              </button>
</form>
          <form accept-charset="UTF-8" action="/Xiaodan/RepData_PeerAssessment2/delete/master/storm_data.md" class="inline-form" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="2FW+sTCS6apvZAvS1FWPt0tPPELMgDk9GInDY5lA+orD8MTP4aey2TwSlcmZkFqSGH8x3dVbeJS1DcKdK9El7g==" /></div>
            <button class="octicon-btn octicon-btn-danger tooltipped tooltipped-n" type="submit" aria-label="Fork this project and delete file" data-disable-with>
              <span class="octicon octicon-trashcan"></span>
            </button>
</form>    </div>

    <div class="file-info">
        305 lines (255 sloc)
        <span class="file-info-divider"></span>
      12.075 kb
    </div>
  </div>
    <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1>
<a id="user-content-reproducible-research-peer-assessment-2" class="anchor" href="#reproducible-research-peer-assessment-2" aria-hidden="true"><span class="octicon octicon-link"></span></a>Reproducible Research: Peer Assessment 2</h1>

<p>Created by Xiaodan Zhang on July 25, 2014</p>

<h2>
<a id="user-content-impact-of-severe-weather-events-on-public-health-and-economy-in-the-united-states" class="anchor" href="#impact-of-severe-weather-events-on-public-health-and-economy-in-the-united-states" aria-hidden="true"><span class="octicon octicon-link"></span></a>Impact of Severe Weather Events on Public Health and Economy in the United States</h2>

<h3>
<a id="user-content-synonpsis" class="anchor" href="#synonpsis" aria-hidden="true"><span class="octicon octicon-link"></span></a>Synonpsis</h3>

<p>In this report, we aim to analyze the impact of different weather events on public health and economy based on the storm database collected from the U.S. National Oceanic and Atmospheric Administration's (NOAA) from 1950 - 2011. We will use the estimates of fatalities, injuries, property and crop damage to decide which types of event are most harmful to the population health and economy. From these data, we found that excessive heat and tornado are most harmful with respect to population health, while flood, drought, and hurricane/typhoon have the greatest economic consequences.</p>

<h3>
<a id="user-content-basic-settings" class="anchor" href="#basic-settings" aria-hidden="true"><span class="octicon octicon-link"></span></a>Basic settings</h3>

<div class="highlight highlight-r"><pre><span class="pl-v">echo</span> <span class="pl-k">=</span> <span class="pl-c1">TRUE</span>  <span class="pl-c"># Always make code visible</span>
options(<span class="pl-v">scipen</span> <span class="pl-k">=</span> <span class="pl-c1">1</span>)  <span class="pl-c"># Turn off scientific notations for numbers</span>
library(<span class="pl-smi">R.utils</span>)
library(<span class="pl-smi">ggplot2</span>)
library(<span class="pl-smi">plyr</span>)
require(<span class="pl-smi">gridExtra</span>)</pre></div>

<h3>
<a id="user-content-data-processing" class="anchor" href="#data-processing" aria-hidden="true"><span class="octicon octicon-link"></span></a>Data Processing</h3>

<p>First, we download the data file and unzip it.</p>

<div class="highlight highlight-r"><pre>setwd(<span class="pl-s"><span class="pl-pds">"</span>~/Desktop/Online Coursera/Coursera-Reproducible-Research/RepData_PeerAssessment2/<span class="pl-pds">"</span></span>)

<span class="pl-k">if</span> (<span class="pl-k">!</span><span class="pl-s"><span class="pl-pds">"</span>stormData.csv.bz2<span class="pl-pds">"</span></span> <span class="pl-k">%in%</span> dir(<span class="pl-s"><span class="pl-pds">"</span>./data/<span class="pl-pds">"</span></span>)) {
    print(<span class="pl-s"><span class="pl-pds">"</span>hhhh<span class="pl-pds">"</span></span>)
    download.file(<span class="pl-s"><span class="pl-pds">"</span>http://d396qusza40orc.cloudfront.net/repdata%2Fdata%2FStormData.csv.bz2<span class="pl-pds">"</span></span>, <span class="pl-v">destfile</span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">"</span>data/stormData.csv.bz2<span class="pl-pds">"</span></span>)
    bunzip2(<span class="pl-s"><span class="pl-pds">"</span>data/stormData.csv.bz2<span class="pl-pds">"</span></span>, <span class="pl-v">overwrite</span><span class="pl-k">=</span><span class="pl-c1">T</span>, <span class="pl-v">remove</span><span class="pl-k">=</span><span class="pl-c1">F</span>)
}</pre></div>

<p>Then, we read the generated csv file. If the data already exists in the working environment, we do not need to load it again. Otherwise, we read the csv file.</p>

<div class="highlight highlight-r"><pre><span class="pl-k">if</span> (<span class="pl-k">!</span><span class="pl-s"><span class="pl-pds">"</span>stormData<span class="pl-pds">"</span></span> <span class="pl-k">%in%</span> ls()) {
    <span class="pl-smi">stormData</span> <span class="pl-k">&lt;-</span> read.csv(<span class="pl-s"><span class="pl-pds">"</span>data/stormData.csv<span class="pl-pds">"</span></span>, <span class="pl-v">sep</span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">"</span>,<span class="pl-pds">"</span></span>)
}
dim(<span class="pl-smi">stormData</span>)</pre></div>

<pre><code>## [1] 902297     38
</code></pre>

<div class="highlight highlight-r"><pre>head(<span class="pl-smi">stormData</span>, <span class="pl-v">n</span> <span class="pl-k">=</span> <span class="pl-c1">2</span>)</pre></div>

<pre><code>##   STATE__          BGN_DATE BGN_TIME TIME_ZONE COUNTY COUNTYNAME STATE
## 1       1 4/18/1950 0:00:00     0130       CST     97     MOBILE    AL
## 2       1 4/18/1950 0:00:00     0145       CST      3    BALDWIN    AL
##    EVTYPE BGN_RANGE BGN_AZI BGN_LOCATI END_DATE END_TIME COUNTY_END
## 1 TORNADO         0                                               0
## 2 TORNADO         0                                               0
##   COUNTYENDN END_RANGE END_AZI END_LOCATI LENGTH WIDTH F MAG FATALITIES
## 1         NA         0                        14   100 3   0          0
## 2         NA         0                         2   150 2   0          0
##   INJURIES PROPDMG PROPDMGEXP CROPDMG CROPDMGEXP WFO STATEOFFIC ZONENAMES
## 1       15    25.0          K       0                                    
## 2        0     2.5          K       0                                    
##   LATITUDE LONGITUDE LATITUDE_E LONGITUDE_ REMARKS REFNUM year
## 1     3040      8812       3051       8806              1 1950
## 2     3042      8755          0          0              2 1950
</code></pre>

<p>There are 902297 rows and 37 columns in total.
The events in the database start in the year 1950 and end in November 2011. In the earlier years of the database there are generally fewer events recorded, most likely due to a lack of good records. More recent years should be considered more complete.</p>

<div class="highlight highlight-r"><pre><span class="pl-k">if</span> (dim(<span class="pl-smi">stormData</span>)[<span class="pl-c1">2</span>] <span class="pl-k">==</span> <span class="pl-c1">37</span>) {
    <span class="pl-smi">stormData</span><span class="pl-k">$</span><span class="pl-smi">year</span> <span class="pl-k">&lt;-</span> as.numeric(format(as.Date(<span class="pl-smi">stormData</span><span class="pl-k">$</span><span class="pl-smi">BGN_DATE</span>, <span class="pl-v">format</span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">"</span>%m/%d/%Y %H:%M:%S<span class="pl-pds">"</span></span>), <span class="pl-s"><span class="pl-pds">"</span>%Y<span class="pl-pds">"</span></span>))
}
hist(<span class="pl-smi">stormData</span><span class="pl-k">$</span><span class="pl-smi">year</span>, <span class="pl-v">breaks</span> <span class="pl-k">=</span> <span class="pl-c1">30</span>)</pre></div>

<p><a href="/Xiaodan/RepData_PeerAssessment2/blob/master/figure/unnamed-chunk-4.png" target="_blank"><img src="/Xiaodan/RepData_PeerAssessment2/raw/master/figure/unnamed-chunk-4.png" alt="plot of chunk unnamed-chunk-4" style="max-width:100%;"></a> </p>

<p>Based on the above histogram, we see that the number of events tracked starts to significantly increase around 1995. So, we use the subset of the data from 1990 to 2011 to get most out of good records.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">storm</span> <span class="pl-k">&lt;-</span> <span class="pl-smi">stormData</span>[<span class="pl-smi">stormData</span><span class="pl-k">$</span><span class="pl-smi">year</span> <span class="pl-k">&gt;</span><span class="pl-k">=</span> <span class="pl-c1">1995</span>, ]
dim(<span class="pl-smi">storm</span>)</pre></div>

<pre><code>## [1] 681500     38
</code></pre>

<p>Now, there are 681500 rows and 38 columns in total.</p>

<h4>
<a id="user-content-impact-on-public-health" class="anchor" href="#impact-on-public-health" aria-hidden="true"><span class="octicon octicon-link"></span></a>Impact on Public Health</h4>

<p>In this section, we check the number of <strong>fatalities</strong> and <strong>injuries</strong> that are caused by the severe weather events. We would like to get the first 15 most severe types of weather events.</p>

<div class="highlight highlight-r"><pre><span class="pl-en">sortHelper</span> <span class="pl-k">&lt;-</span> <span class="pl-k">function</span>(<span class="pl-smi">fieldName</span>, <span class="pl-v">top</span> <span class="pl-k">=</span> <span class="pl-c1">15</span>, <span class="pl-v">dataset</span> <span class="pl-k">=</span> <span class="pl-smi">stormData</span>) {
    <span class="pl-smi">index</span> <span class="pl-k">&lt;-</span> which(colnames(<span class="pl-smi">dataset</span>) <span class="pl-k">==</span> <span class="pl-smi">fieldName</span>)
    <span class="pl-smi">field</span> <span class="pl-k">&lt;-</span> aggregate(<span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>], <span class="pl-v">by</span> <span class="pl-k">=</span> <span class="pl-k">list</span>(<span class="pl-smi">dataset</span><span class="pl-k">$</span><span class="pl-smi">EVTYPE</span>), <span class="pl-v">FUN</span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">"</span>sum<span class="pl-pds">"</span></span>)
    names(<span class="pl-smi">field</span>) <span class="pl-k">&lt;-</span> c(<span class="pl-s"><span class="pl-pds">"</span>EVTYPE<span class="pl-pds">"</span></span>, <span class="pl-smi">fieldName</span>)
    <span class="pl-smi">field</span> <span class="pl-k">&lt;-</span> arrange(<span class="pl-smi">field</span>, <span class="pl-smi">field</span>[, <span class="pl-c1">2</span>], <span class="pl-v">decreasing</span> <span class="pl-k">=</span> <span class="pl-c1">T</span>)
    <span class="pl-smi">field</span> <span class="pl-k">&lt;-</span> head(<span class="pl-smi">field</span>, <span class="pl-v">n</span> <span class="pl-k">=</span> <span class="pl-smi">top</span>)
    <span class="pl-smi">field</span> <span class="pl-k">&lt;-</span> within(<span class="pl-smi">field</span>, <span class="pl-smi">EVTYPE</span> <span class="pl-k">&lt;-</span> <span class="pl-k">factor</span>(<span class="pl-v">x</span> <span class="pl-k">=</span> <span class="pl-smi">EVTYPE</span>, <span class="pl-v">levels</span> <span class="pl-k">=</span> <span class="pl-smi">field</span><span class="pl-k">$</span><span class="pl-smi">EVTYPE</span>))
    <span class="pl-k">return</span>(<span class="pl-smi">field</span>)
}

<span class="pl-smi">fatalities</span> <span class="pl-k">&lt;-</span> sortHelper(<span class="pl-s"><span class="pl-pds">"</span>FATALITIES<span class="pl-pds">"</span></span>, <span class="pl-v">dataset</span> <span class="pl-k">=</span> <span class="pl-smi">storm</span>)
<span class="pl-smi">injuries</span> <span class="pl-k">&lt;-</span> sortHelper(<span class="pl-s"><span class="pl-pds">"</span>INJURIES<span class="pl-pds">"</span></span>, <span class="pl-v">dataset</span> <span class="pl-k">=</span> <span class="pl-smi">storm</span>)</pre></div>

<h4>
<a id="user-content-impact-on-economy" class="anchor" href="#impact-on-economy" aria-hidden="true"><span class="octicon octicon-link"></span></a>Impact on Economy</h4>

<p>We will convert the <strong>property damage</strong> and <strong>crop damage</strong> data into comparable numerical forms according to the meaning of units described in the code book (<a href="http://ire.org/nicar/database-library/databases/storm-events/">Storm Events</a>). Both <code>PROPDMGEXP</code> and <code>CROPDMGEXP</code> columns record a multiplier for each observation where we have Hundred (H), Thousand (K), Million (M) and Billion (B).</p>

<div class="highlight highlight-r"><pre><span class="pl-en">convertHelper</span> <span class="pl-k">&lt;-</span> <span class="pl-k">function</span>(<span class="pl-v">dataset</span> <span class="pl-k">=</span> <span class="pl-smi">storm</span>, <span class="pl-smi">fieldName</span>, <span class="pl-smi">newFieldName</span>) {
    <span class="pl-smi">totalLen</span> <span class="pl-k">&lt;-</span> dim(<span class="pl-smi">dataset</span>)[<span class="pl-c1">2</span>]
    <span class="pl-smi">index</span> <span class="pl-k">&lt;-</span> which(colnames(<span class="pl-smi">dataset</span>) <span class="pl-k">==</span> <span class="pl-smi">fieldName</span>)
    <span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>] <span class="pl-k">&lt;-</span> as.character(<span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>])
    <span class="pl-smi">logic</span> <span class="pl-k">&lt;-</span> <span class="pl-k">!</span>is.na(toupper(<span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>]))
    <span class="pl-smi">dataset</span>[<span class="pl-smi">logic</span> <span class="pl-k">&amp;</span> toupper(<span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>]) <span class="pl-k">==</span> <span class="pl-s"><span class="pl-pds">"</span>B<span class="pl-pds">"</span></span>, <span class="pl-smi">index</span>] <span class="pl-k">&lt;-</span> <span class="pl-s"><span class="pl-pds">"</span>9<span class="pl-pds">"</span></span>
    <span class="pl-smi">dataset</span>[<span class="pl-smi">logic</span> <span class="pl-k">&amp;</span> toupper(<span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>]) <span class="pl-k">==</span> <span class="pl-s"><span class="pl-pds">"</span>M<span class="pl-pds">"</span></span>, <span class="pl-smi">index</span>] <span class="pl-k">&lt;-</span> <span class="pl-s"><span class="pl-pds">"</span>6<span class="pl-pds">"</span></span>
    <span class="pl-smi">dataset</span>[<span class="pl-smi">logic</span> <span class="pl-k">&amp;</span> toupper(<span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>]) <span class="pl-k">==</span> <span class="pl-s"><span class="pl-pds">"</span>K<span class="pl-pds">"</span></span>, <span class="pl-smi">index</span>] <span class="pl-k">&lt;-</span> <span class="pl-s"><span class="pl-pds">"</span>3<span class="pl-pds">"</span></span>
    <span class="pl-smi">dataset</span>[<span class="pl-smi">logic</span> <span class="pl-k">&amp;</span> toupper(<span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>]) <span class="pl-k">==</span> <span class="pl-s"><span class="pl-pds">"</span>H<span class="pl-pds">"</span></span>, <span class="pl-smi">index</span>] <span class="pl-k">&lt;-</span> <span class="pl-s"><span class="pl-pds">"</span>2<span class="pl-pds">"</span></span>
    <span class="pl-smi">dataset</span>[<span class="pl-smi">logic</span> <span class="pl-k">&amp;</span> toupper(<span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>]) <span class="pl-k">==</span> <span class="pl-s"><span class="pl-pds">"</span><span class="pl-pds">"</span></span>, <span class="pl-smi">index</span>] <span class="pl-k">&lt;-</span> <span class="pl-s"><span class="pl-pds">"</span>0<span class="pl-pds">"</span></span>
    <span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>] <span class="pl-k">&lt;-</span> as.numeric(<span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>])
    <span class="pl-smi">dataset</span>[is.na(<span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>]), <span class="pl-smi">index</span>] <span class="pl-k">&lt;-</span> <span class="pl-c1">0</span>
    <span class="pl-smi">dataset</span> <span class="pl-k">&lt;-</span> cbind(<span class="pl-smi">dataset</span>, <span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span> <span class="pl-k">-</span> <span class="pl-c1">1</span>] <span class="pl-k">*</span> <span class="pl-c1">10</span><span class="pl-k">^</span><span class="pl-smi">dataset</span>[, <span class="pl-smi">index</span>])
    names(<span class="pl-smi">dataset</span>)[<span class="pl-smi">totalLen</span> <span class="pl-k">+</span> <span class="pl-c1">1</span>] <span class="pl-k">&lt;-</span> <span class="pl-smi">newFieldName</span>
    <span class="pl-k">return</span>(<span class="pl-smi">dataset</span>)
}

<span class="pl-smi">storm</span> <span class="pl-k">&lt;-</span> convertHelper(<span class="pl-smi">storm</span>, <span class="pl-s"><span class="pl-pds">"</span>PROPDMGEXP<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>propertyDamage<span class="pl-pds">"</span></span>)</pre></div>

<pre><code>## Warning: NAs introduced by coercion
</code></pre>

<div class="highlight highlight-r"><pre><span class="pl-smi">storm</span> <span class="pl-k">&lt;-</span> convertHelper(<span class="pl-smi">storm</span>, <span class="pl-s"><span class="pl-pds">"</span>CROPDMGEXP<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>cropDamage<span class="pl-pds">"</span></span>)</pre></div>

<pre><code>## Warning: NAs introduced by coercion
</code></pre>

<div class="highlight highlight-r"><pre>names(<span class="pl-smi">storm</span>)</pre></div>

<pre><code>##  [1] "STATE__"        "BGN_DATE"       "BGN_TIME"       "TIME_ZONE"     
##  [5] "COUNTY"         "COUNTYNAME"     "STATE"          "EVTYPE"        
##  [9] "BGN_RANGE"      "BGN_AZI"        "BGN_LOCATI"     "END_DATE"      
## [13] "END_TIME"       "COUNTY_END"     "COUNTYENDN"     "END_RANGE"     
## [17] "END_AZI"        "END_LOCATI"     "LENGTH"         "WIDTH"         
## [21] "F"              "MAG"            "FATALITIES"     "INJURIES"      
## [25] "PROPDMG"        "PROPDMGEXP"     "CROPDMG"        "CROPDMGEXP"    
## [29] "WFO"            "STATEOFFIC"     "ZONENAMES"      "LATITUDE"      
## [33] "LONGITUDE"      "LATITUDE_E"     "LONGITUDE_"     "REMARKS"       
## [37] "REFNUM"         "year"           "propertyDamage" "cropDamage"
</code></pre>

<div class="highlight highlight-r"><pre>options(<span class="pl-v">scipen</span><span class="pl-k">=</span><span class="pl-c1">999</span>)
<span class="pl-smi">property</span> <span class="pl-k">&lt;-</span> sortHelper(<span class="pl-s"><span class="pl-pds">"</span>propertyDamage<span class="pl-pds">"</span></span>, <span class="pl-v">dataset</span> <span class="pl-k">=</span> <span class="pl-smi">storm</span>)
<span class="pl-smi">crop</span> <span class="pl-k">&lt;-</span> sortHelper(<span class="pl-s"><span class="pl-pds">"</span>cropDamage<span class="pl-pds">"</span></span>, <span class="pl-v">dataset</span> <span class="pl-k">=</span> <span class="pl-smi">storm</span>)</pre></div>

<h3>
<a id="user-content-results" class="anchor" href="#results" aria-hidden="true"><span class="octicon octicon-link"></span></a>Results</h3>

<p>As for the impact on public health, we have got two sorted lists of severe weather events below by the number of people badly affected.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">fatalities</span></pre></div>

<pre><code>##               EVTYPE FATALITIES
## 1     EXCESSIVE HEAT       1903
## 2            TORNADO       1545
## 3        FLASH FLOOD        934
## 4               HEAT        924
## 5          LIGHTNING        729
## 6              FLOOD        423
## 7        RIP CURRENT        360
## 8          HIGH WIND        241
## 9          TSTM WIND        241
## 10         AVALANCHE        223
## 11      RIP CURRENTS        204
## 12      WINTER STORM        195
## 13         HEAT WAVE        161
## 14 THUNDERSTORM WIND        131
## 15      EXTREME COLD        126
</code></pre>

<div class="highlight highlight-r"><pre><span class="pl-smi">injuries</span></pre></div>

<pre><code>##               EVTYPE INJURIES
## 1            TORNADO    21765
## 2              FLOOD     6769
## 3     EXCESSIVE HEAT     6525
## 4          LIGHTNING     4631
## 5          TSTM WIND     3630
## 6               HEAT     2030
## 7        FLASH FLOOD     1734
## 8  THUNDERSTORM WIND     1426
## 9       WINTER STORM     1298
## 10 HURRICANE/TYPHOON     1275
## 11         HIGH WIND     1093
## 12              HAIL      916
## 13          WILDFIRE      911
## 14        HEAVY SNOW      751
## 15               FOG      718
</code></pre>

<p>And the following is a pair of graphs of total fatalities and total injuries affected by these severe weather events. </p>

<div class="highlight highlight-r"><pre><span class="pl-smi">fatalitiesPlot</span> <span class="pl-k">&lt;-</span> qplot(<span class="pl-smi">EVTYPE</span>, <span class="pl-v">data</span> <span class="pl-k">=</span> <span class="pl-smi">fatalities</span>, <span class="pl-v">weight</span> <span class="pl-k">=</span> <span class="pl-smi">FATALITIES</span>, <span class="pl-v">geom</span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">"</span>bar<span class="pl-pds">"</span></span>, <span class="pl-v">binwidth</span> <span class="pl-k">=</span> <span class="pl-c1">1</span>) <span class="pl-k">+</span> 
    scale_y_continuous(<span class="pl-s"><span class="pl-pds">"</span>Number of Fatalities<span class="pl-pds">"</span></span>) <span class="pl-k">+</span> 
    theme(<span class="pl-v">axis.text.x</span> <span class="pl-k">=</span> element_text(<span class="pl-v">angle</span> <span class="pl-k">=</span> <span class="pl-c1">45</span>, 
    <span class="pl-v">hjust</span> <span class="pl-k">=</span> <span class="pl-c1">1</span>)) <span class="pl-k">+</span> xlab(<span class="pl-s"><span class="pl-pds">"</span>Severe Weather Type<span class="pl-pds">"</span></span>) <span class="pl-k">+</span> 
    ggtitle(<span class="pl-s"><span class="pl-pds">"</span>Total Fatalities by Severe Weather<span class="pl-cce">\n</span> Events in the U.S.<span class="pl-cce">\n</span> from 1995 - 2011<span class="pl-pds">"</span></span>)
<span class="pl-smi">injuriesPlot</span> <span class="pl-k">&lt;-</span> qplot(<span class="pl-smi">EVTYPE</span>, <span class="pl-v">data</span> <span class="pl-k">=</span> <span class="pl-smi">injuries</span>, <span class="pl-v">weight</span> <span class="pl-k">=</span> <span class="pl-smi">INJURIES</span>, <span class="pl-v">geom</span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">"</span>bar<span class="pl-pds">"</span></span>, <span class="pl-v">binwidth</span> <span class="pl-k">=</span> <span class="pl-c1">1</span>) <span class="pl-k">+</span> 
    scale_y_continuous(<span class="pl-s"><span class="pl-pds">"</span>Number of Injuries<span class="pl-pds">"</span></span>) <span class="pl-k">+</span> 
    theme(<span class="pl-v">axis.text.x</span> <span class="pl-k">=</span> element_text(<span class="pl-v">angle</span> <span class="pl-k">=</span> <span class="pl-c1">45</span>, 
    <span class="pl-v">hjust</span> <span class="pl-k">=</span> <span class="pl-c1">1</span>)) <span class="pl-k">+</span> xlab(<span class="pl-s"><span class="pl-pds">"</span>Severe Weather Type<span class="pl-pds">"</span></span>) <span class="pl-k">+</span> 
    ggtitle(<span class="pl-s"><span class="pl-pds">"</span>Total Injuries by Severe Weather<span class="pl-cce">\n</span> Events in the U.S.<span class="pl-cce">\n</span> from 1995 - 2011<span class="pl-pds">"</span></span>)
grid.arrange(<span class="pl-smi">fatalitiesPlot</span>, <span class="pl-smi">injuriesPlot</span>, <span class="pl-v">ncol</span> <span class="pl-k">=</span> <span class="pl-c1">2</span>)</pre></div>

<p><a href="/Xiaodan/RepData_PeerAssessment2/blob/master/figure/unnamed-chunk-9.png" target="_blank"><img src="/Xiaodan/RepData_PeerAssessment2/raw/master/figure/unnamed-chunk-9.png" alt="plot of chunk unnamed-chunk-9" style="max-width:100%;"></a> </p>

<p>Based on the above histograms, we find that <strong>excessive heat</strong> and <strong>tornado</strong> cause most fatalities; <strong>tornato</strong> causes most injuries in the United States from 1995 to 2011.</p>

<p>As for the impact on economy, we have got two sorted lists below by the amount of money cost by damages.  </p>

<div class="highlight highlight-r"><pre><span class="pl-smi">property</span></pre></div>

<pre><code>##               EVTYPE propertyDamage
## 1              FLOOD   144022037057
## 2  HURRICANE/TYPHOON    69305840000
## 3        STORM SURGE    43193536000
## 4            TORNADO    24935939545
## 5        FLASH FLOOD    16047794571
## 6               HAIL    15048722103
## 7          HURRICANE    11812819010
## 8     TROPICAL STORM     7653335550
## 9          HIGH WIND     5259785375
## 10          WILDFIRE     4759064000
## 11  STORM SURGE/TIDE     4641188000
## 12         TSTM WIND     4482361440
## 13         ICE STORM     3643555810
## 14 THUNDERSTORM WIND     3399282992
## 15    HURRICANE OPAL     3172846000
</code></pre>

<div class="highlight highlight-r"><pre><span class="pl-smi">crop</span></pre></div>

<pre><code>##               EVTYPE  cropDamage
## 1            DROUGHT 13922066000
## 2              FLOOD  5422810400
## 3          HURRICANE  2741410000
## 4               HAIL  2614127070
## 5  HURRICANE/TYPHOON  2607872800
## 6        FLASH FLOOD  1343915000
## 7       EXTREME COLD  1292473000
## 8       FROST/FREEZE  1094086000
## 9         HEAVY RAIN   728399800
## 10    TROPICAL STORM   677836000
## 11         HIGH WIND   633561300
## 12         TSTM WIND   553947350
## 13    EXCESSIVE HEAT   492402000
## 14 THUNDERSTORM WIND   414354000
## 15              HEAT   401411500
</code></pre>

<p>And the following is a pair of graphs of total property damage and total crop damage affected by these severe weather events. </p>

<div class="highlight highlight-r"><pre><span class="pl-smi">propertyPlot</span> <span class="pl-k">&lt;-</span> qplot(<span class="pl-smi">EVTYPE</span>, <span class="pl-v">data</span> <span class="pl-k">=</span> <span class="pl-smi">property</span>, <span class="pl-v">weight</span> <span class="pl-k">=</span> <span class="pl-smi">propertyDamage</span>, <span class="pl-v">geom</span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">"</span>bar<span class="pl-pds">"</span></span>, <span class="pl-v">binwidth</span> <span class="pl-k">=</span> <span class="pl-c1">1</span>) <span class="pl-k">+</span> 
    theme(<span class="pl-v">axis.text.x</span> <span class="pl-k">=</span> element_text(<span class="pl-v">angle</span> <span class="pl-k">=</span> <span class="pl-c1">45</span>, <span class="pl-v">hjust</span> <span class="pl-k">=</span> <span class="pl-c1">1</span>)) <span class="pl-k">+</span> scale_y_continuous(<span class="pl-s"><span class="pl-pds">"</span>Property Damage in US dollars<span class="pl-pds">"</span></span>)<span class="pl-k">+</span> 
    xlab(<span class="pl-s"><span class="pl-pds">"</span>Severe Weather Type<span class="pl-pds">"</span></span>) <span class="pl-k">+</span> ggtitle(<span class="pl-s"><span class="pl-pds">"</span>Total Property Damage by<span class="pl-cce">\n</span> Severe Weather Events in<span class="pl-cce">\n</span> the U.S. from 1995 - 2011<span class="pl-pds">"</span></span>)

<span class="pl-smi">cropPlot</span><span class="pl-k">&lt;-</span> qplot(<span class="pl-smi">EVTYPE</span>, <span class="pl-v">data</span> <span class="pl-k">=</span> <span class="pl-smi">crop</span>, <span class="pl-v">weight</span> <span class="pl-k">=</span> <span class="pl-smi">cropDamage</span>, <span class="pl-v">geom</span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">"</span>bar<span class="pl-pds">"</span></span>, <span class="pl-v">binwidth</span> <span class="pl-k">=</span> <span class="pl-c1">1</span>) <span class="pl-k">+</span> 
    theme(<span class="pl-v">axis.text.x</span> <span class="pl-k">=</span> element_text(<span class="pl-v">angle</span> <span class="pl-k">=</span> <span class="pl-c1">45</span>, <span class="pl-v">hjust</span> <span class="pl-k">=</span> <span class="pl-c1">1</span>)) <span class="pl-k">+</span> scale_y_continuous(<span class="pl-s"><span class="pl-pds">"</span>Crop Damage in US dollars<span class="pl-pds">"</span></span>) <span class="pl-k">+</span> 
    xlab(<span class="pl-s"><span class="pl-pds">"</span>Severe Weather Type<span class="pl-pds">"</span></span>) <span class="pl-k">+</span> ggtitle(<span class="pl-s"><span class="pl-pds">"</span>Total Crop Damage by <span class="pl-cce">\n</span>Severe Weather Events in<span class="pl-cce">\n</span> the U.S. from 1995 - 2011<span class="pl-pds">"</span></span>)
grid.arrange(<span class="pl-smi">propertyPlot</span>, <span class="pl-smi">cropPlot</span>, <span class="pl-v">ncol</span> <span class="pl-k">=</span> <span class="pl-c1">2</span>)</pre></div>

<p><a href="/Xiaodan/RepData_PeerAssessment2/blob/master/figure/unnamed-chunk-11.png" target="_blank"><img src="/Xiaodan/RepData_PeerAssessment2/raw/master/figure/unnamed-chunk-11.png" alt="plot of chunk unnamed-chunk-11" style="max-width:100%;"></a> </p>

<p>Based on the above histograms, we find that <strong>flood</strong> and <strong>hurricane/typhoon</strong> cause most property damage; <strong>drought</strong> and <strong>flood</strong> causes most crop damage in the United States from 1995 to 2011.</p>

<h3>
<a id="user-content-conclusion" class="anchor" href="#conclusion" aria-hidden="true"><span class="octicon octicon-link"></span></a>Conclusion</h3>

<p>From these data, we found that <strong>excessive heat</strong> and <strong>tornado</strong> are most harmful with respect to population health, while <strong>flood</strong>, <strong>drought</strong>, and <strong>hurricane/typhoon</strong> have the greatest economic consequences.</p>
</article>
  </div>

</div>

<a href="#jump-to-line" rel="facebox[.linejump]" data-hotkey="l" style="display:none">Jump to Line</a>
<div id="jump-to-line" style="display:none">
  <form accept-charset="UTF-8" class="js-jump-to-line-form">
    <input class="linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" autofocus>
    <button type="submit" class="btn">Go</button>
  </form>
</div>

        </div>

      </div><!-- /.repo-container -->
      <div class="modal-backdrop"></div>
    </div><!-- /.container -->
  </div><!-- /.site -->


    </div><!-- /.wrapper -->

      <div class="container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links right">
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage">
      <span class="mega-octicon octicon-mark-github" title="GitHub"></span>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2015 <span title="0.05681s from github-fe125-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact</a></li>
    </ul>
  </div>
</div>


    <div class="fullscreen-overlay js-fullscreen-overlay" id="fullscreen_overlay">
  <div class="fullscreen-container js-suggester-container">
    <div class="textarea-wrap">
      <textarea name="fullscreen-contents" id="fullscreen-contents" class="fullscreen-contents js-fullscreen-contents" placeholder=""></textarea>
      <div class="suggester-container">
        <div class="suggester fullscreen-suggester js-suggester js-navigation-container"></div>
      </div>
    </div>
  </div>
  <div class="fullscreen-sidebar">
    <a href="#" class="exit-fullscreen js-exit-fullscreen tooltipped tooltipped-w" aria-label="Exit Zen Mode">
      <span class="mega-octicon octicon-screen-normal"></span>
    </a>
    <a href="#" class="theme-switcher js-theme-switcher tooltipped tooltipped-w"
      aria-label="Switch themes">
      <span class="octicon octicon-color-mode"></span>
    </a>
  </div>
</div>



    
    

    <div id="ajax-error-message" class="flash flash-error">
      <span class="octicon octicon-alert"></span>
      <a href="#" class="octicon octicon-x flash-close js-ajax-error-dismiss" aria-label="Dismiss error"></a>
      Something went wrong with that request. Please try again.
    </div>


      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-d22b59d0085e83b7549ba4341ec9e68f80c2f29c8e49213ee182003dc8d568c6.js"></script>
      <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github-0bc0f45c838b5d9d25bc071d2a4b0abe759a093392087dce55cd2caa00ea4f36.js"></script>
      
      

  </body>
</html>
