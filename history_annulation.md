git --no-pager log --oneline  ==>  m�me chose que log, mais sans pagination

git --no-pager log -3 --oneline   ==>  pareil mais n'affiche que les 3 derniers log

git log --since=1.day  ==> affiche les log datant de hier

git log --author "(nom)"  ==> affiche les modifications apport�es par un utilisateur donn�

git log --before="year-month-day"  ==>  affiche tous les log apr�s une date donn�e

git log file_name.file_type  ==>  affiche tous les log qui ont un rapport avec un fichier donn�

git log -p file_name.file_type ==>  affiche toutes les modifications apport�es au fichier � chaque commit

git log -p  ==> affiche toutes les modifications apport�es � tous les fichiers � chaque commit

git log -2 -p  ==>  affiche les modifications apport�es aux fichiers dans les 2 derniers commits

git --stat file_name.file_type  ==>  affiche les ajouts et les suppressions de lignes dans un fichier donn�

git log -E -i --grep='mot'  ==>  recherhe un log o� on retrouve le mot en question. -E trouve les occurences et -i ignore les majuscules/minuscules

git diff  ==>  montre les diff�rences dans tous les fichiers

git diff --cached  ==>  montre les diff�rences entre le dernier commit et l'index. si on fait add, diff n'affichera rien

git log (ref commit) (ref commit2)  ==>  montre les log entre 2 commits.

git diff --stat  ==>  montre les diff�rences dans tous les fichiers

git restore file_name.file_type  ==>  annule la derni�re action faite � ce fichier

git restore --staged  ==>  si le fichier est dans l'index

git commit "(message)" --amend --no-edit  ==>  modifie uniquement le message du dernier commit

git reset ( )  ==>  supprime le dernier commit d'un fichier

git reset --soft  ==>  garde les commit

git reset --hard  ==> supprime tous les commit (et les modifs par cons�quence )

git checkout (ref commit) file_name.file_type  ==>  modifie le fichier pour qu'il revienne � l'�tat du commit d�sign�

mkdir file_name  ==>  Cr�ation de dossier (vide)

cd file_name  ==>  d�place le module git vers un dossier d�sign�. Necessite les origines si dans un dossier diff�rent.

git revert (ref commit)  ==>  annule toute modification effectu�e depuis le commit en question. Garde les commit d'avant.