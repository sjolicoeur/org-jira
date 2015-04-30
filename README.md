* org-jira Spacemacs layer

This Spacemacs layer allows using Jira from within org-mode.

** Installation

1. Clone the git repository somewhere and add it as a private layer
#+BEGIN_EXAMPLE
	git clone git@github.com:jfim/org-jira.git
	ln -s "`pwd`/org-jira" ~/.emacs.d/private/org-jira
#+END_EXAMPLE

2. Add the =org-jira= layer to your .spacemacs file
3. Add the Jira url to your .spacemacs file. For example, if your Jira is installed at https://example:443/secure/Dashboard.jspa
#+BEGIN_EXAMPLE
(setq jiralib-url "https://example:443")
#+END_EXAMPLE

** Usage

When in org-mode:

<kbd>mjpg</kbd> 'org-jira-get-projects
<kbd>mjib</kbd> 'org-jira-browse-issue
<kbd>mjig</kbd> 'org-jira-get-issues
<kbd>mjih</kbd> 'org-jira-get-issues-headonly
<kbd>mjif</kbd> 'org-jira-get-issues-from-filter-headonly
<kbd>mjiF</kbd> 'org-jira-get-issues-from-filter
<kbd>mjiu</kbd> 'org-jira-update-issue
<kbd>mjiw</kbd> 'org-jira-progress-issue
<kbd>mjir</kbd> 'org-jira-refresh-issue
<kbd>mjic</kbd> 'org-jira-create-issue
<kbd>mjik</kbd> 'org-jira-copy-current-issue-key
<kbd>mjsc</kbd> 'org-jira-create-subtask
<kbd>mjsg</kbd> 'org-jira-get-subtasks
<kbd>mjcu</kbd> 'org-jira-update-comment
<kbd>mjtj</kbd> 'org-jira-todo-to-jira