---
title: LLDB abbreviation translations
date: 2024-04-18T15:00:43.138Z
description: A reference for future me
slug: lldb-abbr-trans
draft: false
---
| Abbreviation | Full form | 
|-|-|
| attach | _regexp-attach |
| b | _regexp-break |
| bt | _regexp-bt |
| display | _regexp-display |
| down | _regexp-down |
| env | _regexp-env |
| jump | _regexp-jump |
| list | _regexp-list |
| tbreak | _regexp-tbreak |
| undisplay | _regexp-undisplay |
| up | _regexp-up |
| rbreak | breakpoint set -r %1 |
| dis | disassemble |
| call | expression -- |
| p | expression -- |
| po | expression -O  -- |
| poarray | expression -O -Z %1    -- |
| parray | expression -Z %1   -- |
| f | frame select |
| var | frame variable |
| x | memory read |
| shell | platform shell -h   -- |
| c | process continue |
| continue | process continue |
| detach | process detach |
| kill | process kill |
| r | process launch -c /bin/bash -- |
| exit | quit |
| q | quit |
| re | register |
| history | session history |
| file | target create |
| image | target modules |
| add-dsym | target symbols add |
| t | thread select |
| sif | thread step-in -e block -t %1 |
| step | thread step-in |
| si | thread step-inst |
| ni | thread step-inst-over |
| finish | thread step-out |
| next | thread step-over |