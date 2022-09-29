# Modelagem do Banco de Dados
Repositório para modelagem do banco de dados

<div align="center">
  <img src="Lógico_1.png"/>
</div>

# Descrição das tabelas do modelo

<h2>Tabela <i>Aluno</i></h2>
A tabela <i>aluno</i> descreve dentro no modelo relacional elaborado, onde e quais atributos iremos manter no banco
sobre dos alunos, no banco de dados da Universidade.
Nela possuímos os atributos/colunas:
<ul>
    <p>MAT : Chave primária da tabela.</p>
    <p>nome :Nome de cada aluno.</p>
    <p>cidade: cidade em que o aluno nasceu.</p>
</ul>

<h2>Tabela <i>Disciplinas</i></h2>
A tabela <i>aluno</i> descreve dentro no modelo relacional elaborado, onde e quais atributos iremos manter no banco
sobre as disciplinas, no banco de dados da Universidade.
<ul>
  <p>cod_disc :Chave primária da tabela.</p>
    <p>nome_disc : Nome da disciplina.</p>
    <p>carga_hor : Carga horária das disciplinas.</p>
</ul>

<h2>Tabela <i> Professores</i></h2>
A tabela <i>aluno</i> descreve dentro no modelo relacional elaborado, onde e quais atributos iremos manter no banco
sobre dos professores, no banco de dados da Universidade.
<ul>
  <p>cod_prof : Chave primária da tabela.</p>
    <p>nome : Nome do professor</p>
    <p>endereco : o endereço do professor</p>
    <p>cidade : cidade em que o professor nasceu.</p>
 </ul>
 
<h2>Tabela <i> varios</i></h2>
A tabela <i>aluno</i> descreve dentro no modelo relacional elaborado, é responsavel por manter de relacionar as tabelas "professores" e  "turma", no banco de dados da Universidade.
<ul>
    <p>fk_alunos_Mat : Chave estrangeira responsavel por fazer referência a tabela de aluno.</p>
    <p>fk_Disciplinas_Cod_Disc : Chave estrangeira responsal por fazer referência a tabela disciplina.</p>
</ul>

<h2>Tabela <i>Histórico</i></h2>
A tabela <i>aluno</i> descreve dentro no modelo relacional elaborado, onde e quais atributos iremos manter no banco
sobre dos alunos, no banco de dados da Universidade.
<ul>
    <p>MAT : Responvesal por fazer referência a matricula do aluno references aluno(MAT).</p>
    <p>ano : responsavel por armazenar o ano em que o aluno está estudando no momento</p>
    <p>cod_disc : responsavel por fazer referência a tabela de disciplinas references discplinas(cod_prof).</p>
    <p>cod_prof : responsavel por fazer referência a tabela de professores references professores(cod_prof).</p>
    <p>cod_turma : responsal por fazer referência a tabela turma references aluno(cod_turma).</p>
    <p>frequencia : Responsavel por armazenar a frequencia do aluno</p>
    <p>nota : Responsavel por armazenar do périodo em que o aluno está na universidade</p>
</ul>
<h2>Tabela <i>Turma</i></h2>
A tabela <i>turma</i> descreve dentro no modelo relacional elaborado, onde e quais atributos iremos manter no banco
sobre dos alunos, no banco de dados da Universidade.
<ul>
    <p>cod_disc : responsavel por fazer referência a tabela de disciplinas references discplinas(cod_prof).</p>
    <p>cod_prof : responsavel por fazer referência a tabela de professores references professores(cod_prof).</p>
    <p>cod_turma : responsal por fazer referência a tabela turma references aluno(cod_turma).</p>
    <p>frequencia : Frequencia dos alunos</p>
    <p>horario : Horarios das turmas</p>
</ul>
