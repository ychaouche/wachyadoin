# Wachyadoin
Every 30 minutes, a dialog box asks you "whachyadoin" and records that in daily log files in ~/NOTES/LOG/.

## Usage
To use wachyadoin, simply invoke it from the command line and run in background

```
$ chmod +x wachyadoin
$ ./wachyadoin &
```

## Add to autostart
You can launch this as soon as you open your DE session by adding it to your personal Autostart folder. In KDE it is ~/.kde/Autostart

```
ychaouche@ychaouche-PC 09:46:31 ~/.kde/Autostart $ ls                                                                                                                                                                                                                          
total 0                                                                                                                                                                                                                                                                        
lrwxrwxrwx 1 ychaouche ychaouche 34 Nov 30 09:39 wachyadoin -> /home/ychaouche/SCRIPTS/wachyadoin                                                                                                                                                                              
ychaouche@ychaouche-PC 09:46:31 ~/.kde/Autostart $  
```

This is useful because you might forget to launch the script when your first login. 

## Background
When you log your activities, at the end of the day, week, month, you can easily see where you put your efforts, where you wasted time, what was that URL again ? oh, if only I have saved it somewhere...

If you wait till the end of your workday to record your thoughts or what you've been working on today, you may not remember all the details. This is where wachyadoin comes in handy : while you're at the task, it will act as a reminder to log anything that might be worth to remember.

So simple, yet so useful.

## Integration with howm-mode

You can configure emacs' howm-mode to easily and effectively search and "wikify" your notes by adding these lines in your .emacs

```
; howm-mode :)
;; search other directories in addition to `howm-directory'.
(setq howm-search-path '("~/NOTES/LOG/"))
(setq howm-search-other-dir t)
```

