+++
title = '{{ replace .File.ContentBaseName "-" " " | title }}'
# the title after the pipe is to change the content to title case
date = {{ .Date }}
draft = false
description = ""
+++
