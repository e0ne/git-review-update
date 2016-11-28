# Simple Plugin for git-review

According to [OpenStack Developer’s Guide](http://docs.openstack.org/infra/manual/developers.html)
you have to use [git-review](http://docs.openstack.org/infra/manual/developers.html#installing-git-review)
to work with Gerrit workflow.

'If the code review process suggests additional changes, make and amend the
changes to the existing commit. To simplify this workflow you can use
'git-review-update' plugin.

## Installation
``` 
sudo wget https://raw.githubusercontent.com/e0ne/git-review-update/master/git-review-update -O /usr/local/bin/git-review-update
sudo chmod +x /usr/local/bin/git-review-update
```

## Usage
In your git repository directory type the following command:
``` git review-update ```

It will invoke ``` git commit -a --amend && git review ```
