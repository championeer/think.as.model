# Doom Emacs Configuration

![rw-book-cover](https://tecosaur.com/resources/org/nib.png)

## Metadata
- Author: [[tecosaur]]
- Full Title: Doom Emacs Configuration
- Category: #articles
- Summary: The Methods, Management, and Menagerie of Madness
- URL: https://tecosaur.github.io/emacs-config/config.html

## Highlights
- Emacs Lisp
  [#](https://tecosaur.github.io/emacs-config/config.html#rudimentary-configuration,code--1) ⎘
  ﻿;﻿;; config.el -*- lexical-binding: t; -*- ([View Highlight](https://read.readwise.io/read/01gp8xfhq6jhn9kp45pys9xy8p))
- Emacs Lisp
  [#](https://tecosaur.github.io/emacs-config/config.html#rudimentary-configuration,code--1) ⎘ ([View Highlight](https://read.readwise.io/read/01gp8xfy0kxxgrwt1m9h7fed75))
- ;﻿;; config.el -*- lexical-binding: t; -*- ([View Highlight](https://read.readwise.io/read/01gp8xg1ar3tqh003mte0qa7da))
- (setq-default delete-by-moving-to-trash t ; Delete files to trash window-combination-resize t ; take new window space from all other windows (not just current) ([View Highlight](https://read.readwise.io/read/01gpjjywkxmsjb8s80am29nysf))
- Emacs Lisp
  [#](https://tecosaur.github.io/emacs-config/config.html#avy,code--1) ⎘
  (after! avy
  ;; home row priorities: 8 6 4 5 - - 1 2 3 7
  (setq avy-keys '(?n ?e ?i ?s ?t ?r ?i ?a))) ([View Highlight](https://read.readwise.io/read/01gp8qnav1axxa90qybjypq325))
- Emacs Lisp
  [#](https://tecosaur.github.io/emacs-config/config.html#keycast,code--2) ⎘
  (use-package! keycast
  :commands keycast-mode
  :config
  (define-minor-mode keycast-mode
  "Show current command and its key binding in the mode line."
  :global t
  (if keycast-mode
  (progn
  (add-hook 'pre-command-hook 'keycast--update t)
  (add-to-list 'global-mode-string '("" mode-line-keycast " ")))
  (remove-hook 'pre-command-hook 'keycast--update)
  (setq global-mode-string (remove '("" mode-line-keycast " ") global-mode-string))))
  (custom-set-faces!
  '(keycast-command :inherit doom-modeline-debug
  :height 0.9)
  '(keycast-key :inherit custom-modified
  :height 1.1
  :weight bold))) ([View Highlight](https://read.readwise.io/read/01gp18k4214rnpsx38n2fktpae))
- (use-package! keycast :commands keycast-mode :config (define-minor-mode keycast-mode "Show current command and its key binding in the mode line." :global t (if keycast-mode (progn (add-hook 'pre-command-hook 'keycast--update t) (add-to-list 'global-mode-string '("" mode-line-keycast " "))) (remove-hook 'pre-command-hook 'keycast--update) (setq global-mode-string (remove '("" mode-line-keycast " ") global-mode-string)))) (custom-set-faces! '(keycast-command :inherit doom-modeline-debug :height 0.9) '(keycast-key :inherit custom-modified :height 1.1 :weight bold))) ([View Highlight](https://read.readwise.io/read/01gp18kkd05jvn0d05psh69ggb))
# Doom Emacs Configuration

![rw-book-cover](https://tecosaur.com/resources/org/nib.png)

## Metadata
- Author: [[tecosaur]]
- Full Title: Doom Emacs Configuration
- Category: #articles
- Summary: The Methods, Management, and Menagerie of Madness
- URL: https://tecosaur.github.io/emacs-config/config.html

## Highlights
- Emacs Lisp
  [#](https://tecosaur.github.io/emacs-config/config.html#rudimentary-configuration,code--1) ⎘
  ﻿;﻿;; config.el -*- lexical-binding: t; -*- ([View Highlight](https://read.readwise.io/read/01gp8xfhq6jhn9kp45pys9xy8p))
- Emacs Lisp
  [#](https://tecosaur.github.io/emacs-config/config.html#rudimentary-configuration,code--1) ⎘ ([View Highlight](https://read.readwise.io/read/01gp8xfy0kxxgrwt1m9h7fed75))
- ;﻿;; config.el -*- lexical-binding: t; -*- ([View Highlight](https://read.readwise.io/read/01gp8xg1ar3tqh003mte0qa7da))
- (setq-default delete-by-moving-to-trash t ; Delete files to trash window-combination-resize t ; take new window space from all other windows (not just current) ([View Highlight](https://read.readwise.io/read/01gpjjywkxmsjb8s80am29nysf))
- Emacs Lisp
  [#](https://tecosaur.github.io/emacs-config/config.html#avy,code--1) ⎘
  (after! avy
  ;; home row priorities: 8 6 4 5 - - 1 2 3 7
  (setq avy-keys '(?n ?e ?i ?s ?t ?r ?i ?a))) ([View Highlight](https://read.readwise.io/read/01gp8qnav1axxa90qybjypq325))
- Emacs Lisp
  [#](https://tecosaur.github.io/emacs-config/config.html#keycast,code--2) ⎘
  (use-package! keycast
  :commands keycast-mode
  :config
  (define-minor-mode keycast-mode
  "Show current command and its key binding in the mode line."
  :global t
  (if keycast-mode
  (progn
  (add-hook 'pre-command-hook 'keycast--update t)
  (add-to-list 'global-mode-string '("" mode-line-keycast " ")))
  (remove-hook 'pre-command-hook 'keycast--update)
  (setq global-mode-string (remove '("" mode-line-keycast " ") global-mode-string))))
  (custom-set-faces!
  '(keycast-command :inherit doom-modeline-debug
  :height 0.9)
  '(keycast-key :inherit custom-modified
  :height 1.1
  :weight bold))) ([View Highlight](https://read.readwise.io/read/01gp18k4214rnpsx38n2fktpae))
- (use-package! keycast :commands keycast-mode :config (define-minor-mode keycast-mode "Show current command and its key binding in the mode line." :global t (if keycast-mode (progn (add-hook 'pre-command-hook 'keycast--update t) (add-to-list 'global-mode-string '("" mode-line-keycast " "))) (remove-hook 'pre-command-hook 'keycast--update) (setq global-mode-string (remove '("" mode-line-keycast " ") global-mode-string)))) (custom-set-faces! '(keycast-command :inherit doom-modeline-debug :height 0.9) '(keycast-key :inherit custom-modified :height 1.1 :weight bold))) ([View Highlight](https://read.readwise.io/read/01gp18kkd05jvn0d05psh69ggb))
