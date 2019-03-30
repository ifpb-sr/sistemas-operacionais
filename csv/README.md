# Trabalhando com arquivos csv


        for t in `cat turmas-2019-abril.csv  | cut -f 1 -d , | uniq` ; do echo Turm,Nome > $t.csv && cat turmas-2019-abril.csv | grep $t >> $t.csv ; done

Queria criar um arquivo para cada turma.
