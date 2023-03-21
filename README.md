# ejerciciosGitHub

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git
$ git init
Initialized empty Git repository in S:/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git/.git/

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        indice.txt

nothing added to commit but untracked files present (use "git add" to track)

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git add indice.txt

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   indice.txt


Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git commit -m "Añadido índice del libro"
[master (root-commit) bdc334c] Añadido índice del libro
 1 file changed, 3 insertions(+)
 create mode 100644 indice.txt

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git status
On branch master
nothing to commit, working tree clean

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git commit -m "Añadido capitulo 3 sobre gestión de ramas"
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   indice.txt

no changes added to commit (use "git add" and/or "git commit -a")

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git commit -a "Añadido capitulo 3 sobre gestión de ramas"
fatal: paths 'Añadido capitulo 3 sobre gestión de ramas ...' with -a does not make sense

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   indice.txt

no changes added to commit (use "git add" and/or "git commit -a")

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git log
commit bdc334cf1c773f205e9d014f14cbd28723f8ed3f (HEAD -> master)
Author: SergioAlmagre <127857356+SergioAlmagre@users.noreply.github.com>
Date:   Tue Mar 21 13:16:20 2023 +0100

    Añadido índice del libro

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git commit -m "Añadido capitulo 3 sobre gestión de ramas"
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   indice.txt

no changes added to commit (use "git add" and/or "git commit -a")

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git commit -m "Añadido capitulo 3 sobre gestión de ramas"^C

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git add indice.txt

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git commit -m "Añadido capitulo 3 sobre gestión de ramas"
[master b5016fe] Añadido capitulo 3 sobre gestión de ramas
 1 file changed, 2 insertions(+), 1 deletion(-)

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git log
commit b5016fe749ba0f08844731c118f8c5985adbf172 (HEAD -> master)
Author: SergioAlmagre <127857356+SergioAlmagre@users.noreply.github.com>
Date:   Tue Mar 21 13:24:47 2023 +0100

    Añadido capitulo 3 sobre gestión de ramas

commit bdc334cf1c773f205e9d014f14cbd28723f8ed3f
Author: SergioAlmagre <127857356+SergioAlmagre@users.noreply.github.com>
Date:   Tue Mar 21 13:16:20 2023 +0100

    Añadido índice del libro

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git add indice.txt

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git commit --amend
[master fe7dd60] Añadido capitulo 3 sobre gestión de ramas modificado
 Date: Tue Mar 21 13:24:47 2023 +0100
 1 file changed, 2 insertions(+), 1 deletion(-)

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git log
commit fe7dd60274b47800008151cefe2b35e1a74b6895 (HEAD -> master)
Author: SergioAlmagre <127857356+SergioAlmagre@users.noreply.github.com>
Date:   Tue Mar 21 13:24:47 2023 +0100

    Añadido capitulo 3 sobre gestión de ramas modificado

commit bdc334cf1c773f205e9d014f14cbd28723f8ed3f
Author: SergioAlmagre <127857356+SergioAlmagre@users.noreply.github.com>
Date:   Tue Mar 21 13:16:20 2023 +0100

    Añadido índice del libro

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ ^C

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git diff fe7dd60274b47800008151cefe2b35e1a74b6895

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git diff  fe7dd60274b47800008151cefe2b35e1a74b6895

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git diff commit fe7dd60274b47800008151cefe2b35e1a74b6895
fatal: ambiguous argument 'commit': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git diff bdc334cf1c773f205e9d014f14cbd28723f8ed3f
diff --git a/indice.txt b/indice.txt
index 0c23e42..b732097 100644
--- a/indice.txt
+++ b/indice.txt
@@ -1,3 +1,4 @@
 Capitulo 1: Introducción a Git
 Capitulo 2: Flujo de trabajo báisco
-Capitulo 3: Repositorios remotos
\ No newline at end of file
+Capitulo 3: Gestión de ramas
+Capitulo 4: Repositorios remotos

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git status
On branch master
nothing to commit, working tree clean

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git log
commit fe7dd60274b47800008151cefe2b35e1a74b6895 (HEAD -> master)
Author: SergioAlmagre <127857356+SergioAlmagre@users.noreply.github.com>
Date:   Tue Mar 21 13:24:47 2023 +0100

    Añadido capitulo 3 sobre gestión de ramas modificado

commit bdc334cf1c773f205e9d014f14cbd28723f8ed3f
Author: SergioAlmagre <127857356+SergioAlmagre@users.noreply.github.com>
Date:   Tue Mar 21 13:16:20 2023 +0100

    Añadido índice del libro

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git push
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using

    git remote add <name> <url>

and then push using the remote name

    git push <name>


Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git remote add
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from


Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git init
Reinitialized existing Git repository in S:/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git/.git/

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git remote add https://github.com/SergioAlmagre/ejerciciosGitHub.git
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from


Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git remote add ejercicios https://github.com/SergioAlmagre/ejerciciosGitHub.git

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ push
bash: push: command not found

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream ejercicios master

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git push --set-upstream ejercicios master
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 603 bytes | 301.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), done.
remote:
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/SergioAlmagre/ejerciciosGitHub/pull/new/master
remote:
To https://github.com/SergioAlmagre/ejerciciosGitHub.git
 * [new branch]      master -> master
branch 'master' set up to track 'ejercicios/master'.

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git clone
fatal: You must specify a repository to clone.

usage: git clone [<options>] [--] <repo> [<dir>]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --progress            force progress reporting
    --reject-shallow      don't clone shallow repository
    -n, --no-checkout     don't create a checkout
    --bare                create a bare repository
    --mirror              create a mirror repository (implies bare)
    -l, --local           to clone from a local repository
    --no-hardlinks        don't use local hardlinks, always copy
    -s, --shared          setup as shared repository
    --recurse-submodules[=<pathspec>]
                          initialize submodules in the clone
    --recursive ...       alias of --recurse-submodules
    -j, --jobs <n>        number of submodules cloned in parallel
    --template <template-directory>
                          directory from which templates will be used
    --reference <repo>    reference repository
    --reference-if-able <repo>
                          reference repository
    --dissociate          use --reference only while cloning
    -o, --origin <name>   use <name> instead of 'origin' to track upstream
    -b, --branch <branch>
                          checkout <branch> instead of the remote's HEAD
    -u, --upload-pack <path>
                          path to git-upload-pack on the remote
    --depth <depth>       create a shallow clone of that depth
    --shallow-since <time>
                          create a shallow clone since a specific time
    --shallow-exclude <revision>
                          deepen history of shallow clone, excluding rev
    --single-branch       clone only one branch, HEAD or --branch
    --no-tags             don't clone any tags, and make later fetches not to follow them
    --shallow-submodules  any cloned submodules will be shallow
    --separate-git-dir <gitdir>
                          separate git dir from working tree
    -c, --config <key=value>
                          set config inside the new repository
    --server-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only
    --filter <args>       object filtering
    --also-filter-submodules
                          apply partial clone filters to submodules
    --remote-submodules   any cloned submodules will use their remote-tracking branch
    --sparse              initialize sparse-checkout file to include only files at root
    --bundle-uri <uri>    a URI for downloading bundles before fetching from origin remote


Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$ git clone https://github.com/SergioAlmagre/ejerciciosGitHub.git
Cloning into 'ejerciciosGitHub'...
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 9 (delta 2), reused 6 (delta 2), pack-reused 0
Receiving objects: 100% (9/9), done.
Resolving deltas: 100% (2/2), done.

Sergio@HP-SERGIO MINGW64 /s/Mi unidad/1ºDAM/3 - Entornos de desarrollo/Tema 4/Actividad Git (master)
$
