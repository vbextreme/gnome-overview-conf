# gnome-overview-conf v0.9
edit gnome overview setting</br>

Released under GPL v3

## Revision
0.10 fix regex same problem v0.9</br>
0.9 fix regex problems for old perl version</br>
0.8 fix backup for distro that not use lib64</br>
0.7 fix type property in library some distro use var instead of const</br>
0.6 fix check lib64 or lib32, discharge gbus error</br>
0.5 fix shebang, fix directory lib is different in some distro</br>
0.4 fix import not reload value, fix formatting export, add theme and screenshot</br>
0.3 fix crash shell</br>
0.2 separate backup, add import and export, fix not save</br>
0.1 code style and initial support for built-in Adwaita theme</br>

## How To
### Install
```
$ git clone https://github.com/vbextreme/gnome-overview-conf.git
$ cd gnome-overview-conf
$ sudo ./install
```

### Uninstall
```
$ sudo ./uninstall
```

### Usage
for view all command</br>
```
$ gnome-overview-conf help
```
create backup for prevent problems</br>
```
$ sudo gnome-overview-conf backup
```
restore backup, save you</br>
```
$ sudo gnome-overview-conf restore
```
view current configuration</br>
```
$ gnome-overview-conf view
```
set one or more value</br>
```
$ sudo gnome-overview-conf max_columns 10 min_rows 5 icon_size 64 horizontal 112 vertical 120
```
after setting value reload shell with</br>
```
ALT+F2 
r
```
go to directory ./theme</br>
save current overview theme, example name mytheme</br>
```
$ sudo gnome-overview-conf export mytheme
```
go to directory ./theme</br>
import theme, example default</br>
```
$ sudo gnome-overview-conf import default
```
