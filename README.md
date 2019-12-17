# kctx

## Overview
This is the context switch helper for kubernetes.  
Enable access to multiple clusters by using tmux pain etc.


## Usage
```
$ # pain 1
$ kctx -h
This is the context switch helper for kubernetes.

usage:
  kctx           : show context list or use peco to filter context
  kctx <NAME>    : switch to <NAME> context

  kctx -h        : show this message

$ kctx dev
$ kubectl config current-context
dev
$ kubectl get pods
~ get dev pod list ~


=== other pain(tmux etc..) ===

$ # pain 2
$ kctx stg
$ kubectl config current-context
stg
$ kubectl get pods
~ get stg pod list ~
```
^^ Example of simultaneous connection to two clusters


## Install
```
$ git clone https://github.com/m3y/kctx.git
$ alias kctx="source /path/to/kctx/kctx"
```
