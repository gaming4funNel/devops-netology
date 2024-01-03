1.
Найти полный хеш и комментарий коммита, хеш которого начинается на aefea:
```
git show aefea
```
```
commit aefead2207ef7e2aa5dc81a34aedf0cad4c32545
Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
Date:   Thu Jun 18 10:29:58 2020 -0400

Update CHANGELOG.md
```
2.
Какому тегу соответствует коммит 85024d3:
```
git describe --tags 85024d3
```
```
v0.12.23
```

Сколько родителей у коммита b8d720 и их хеши:
```
git show --pretty=%P --quiet b8d720
```
```
56cd7859e05c36c06b56d013b55a252d0bb7e158 9ea88f22fc6269854151c571162c5bcf958bee2b
```

Перечислите хеши и комментарии всех коммитов между тегами v0.12.23 и v0.12.24:
```
git log --oneline v0.12.23..v0.12.24
```
```
33ff1c03bb (tag: v0.12.24) v0.12.24
b14b74c493 [Website] vmc provider links
3f235065b9 Update CHANGELOG.md
6ae64e247b registry: Fix panic when server is unreachable
5c619ca1ba website: Remove links to the getting started guide's old location
06275647e2 Update CHANGELOG.md
d5f9411f51 command: Fix bug when using terraform login on Windows
4b6d06cc5d Update CHANGELOG.md
dd01a35078 Update CHANGELOG.md
225466bc3e Cleanup after v0.12.23 release
```

Найти коммит, в котором была создана функция func providerSource:
```
git log -S 'func providerSource' --oneline
```
```
5af1e6234a main: Honor explicit provider_installation CLI config when present
8c928e8358 main: Consult local directories as potential mirrors of providers
```

Найти все коммиты, в которых была изменена функция globalPluginDirs:
```
git log -S 'func globalPluginDirs' --oneline
```
```
8364383c35 Push plugin discovery down into command package
```

Кто автор функции synchronizedWriters:
```
git log -S 'func synchronizedWriters' --pretty="%an" -1
```
```
James Bardin
```
