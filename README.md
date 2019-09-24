"# PHP-aula06-ex5" 
<?xml version="1.0" encoding="utf-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" lang="en" xml:lang="en">
<head>
<!-- 2019-09-23 seg 21:07 -->
<meta http-equiv="Content-Type" content="text/html;charset=utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>&lrm;</title>
<meta name="generator" content="Org mode" />
<style type="text/css">
 <!--/*--><![CDATA[/*><!--*/
  .title  { text-align: center;
             margin-bottom: .2em; }
  .subtitle { text-align: center;
              font-size: medium;
              font-weight: bold;
              margin-top:0; }
  .todo   { font-family: monospace; color: red; }
  .done   { font-family: monospace; color: green; }
  .priority { font-family: monospace; color: orange; }
  .tag    { background-color: #eee; font-family: monospace;
            padding: 2px; font-size: 80%; font-weight: normal; }
  .timestamp { color: #bebebe; }
  .timestamp-kwd { color: #5f9ea0; }
  .org-right  { margin-left: auto; margin-right: 0px;  text-align: right; }
  .org-left   { margin-left: 0px;  margin-right: auto; text-align: left; }
  .org-center { margin-left: auto; margin-right: auto; text-align: center; }
  .underline { text-decoration: underline; }
  #postamble p, #preamble p { font-size: 90%; margin: .2em; }
  p.verse { margin-left: 3%; }
  pre {
    border: 1px solid #ccc;
    box-shadow: 3px 3px 3px #eee;
    padding: 8pt;
    font-family: monospace;
    overflow: auto;
    margin: 1.2em;
  }
  pre.src {
    position: relative;
    overflow: visible;
    padding-top: 1.2em;
  }
  pre.src:before {
    display: none;
    position: absolute;
    background-color: white;
    top: -10px;
    right: 10px;
    padding: 3px;
    border: 1px solid black;
  }
  pre.src:hover:before { display: inline;}
  /* Languages per Org manual */
  pre.src-asymptote:before { content: 'Asymptote'; }
  pre.src-awk:before { content: 'Awk'; }
  pre.src-C:before { content: 'C'; }
  /* pre.src-C++ doesn't work in CSS */
  pre.src-clojure:before { content: 'Clojure'; }
  pre.src-css:before { content: 'CSS'; }
  pre.src-D:before { content: 'D'; }
  pre.src-ditaa:before { content: 'ditaa'; }
  pre.src-dot:before { content: 'Graphviz'; }
  pre.src-calc:before { content: 'Emacs Calc'; }
  pre.src-emacs-lisp:before { content: 'Emacs Lisp'; }
  pre.src-fortran:before { content: 'Fortran'; }
  pre.src-gnuplot:before { content: 'gnuplot'; }
  pre.src-haskell:before { content: 'Haskell'; }
  pre.src-hledger:before { content: 'hledger'; }
  pre.src-java:before { content: 'Java'; }
  pre.src-js:before { content: 'Javascript'; }
  pre.src-latex:before { content: 'LaTeX'; }
  pre.src-ledger:before { content: 'Ledger'; }
  pre.src-lisp:before { content: 'Lisp'; }
  pre.src-lilypond:before { content: 'Lilypond'; }
  pre.src-lua:before { content: 'Lua'; }
  pre.src-matlab:before { content: 'MATLAB'; }
  pre.src-mscgen:before { content: 'Mscgen'; }
  pre.src-ocaml:before { content: 'Objective Caml'; }
  pre.src-octave:before { content: 'Octave'; }
  pre.src-org:before { content: 'Org mode'; }
  pre.src-oz:before { content: 'OZ'; }
  pre.src-plantuml:before { content: 'Plantuml'; }
  pre.src-processing:before { content: 'Processing.js'; }
  pre.src-python:before { content: 'Python'; }
  pre.src-R:before { content: 'R'; }
  pre.src-ruby:before { content: 'Ruby'; }
  pre.src-sass:before { content: 'Sass'; }
  pre.src-scheme:before { content: 'Scheme'; }
  pre.src-screen:before { content: 'Gnu Screen'; }
  pre.src-sed:before { content: 'Sed'; }
  pre.src-sh:before { content: 'shell'; }
  pre.src-sql:before { content: 'SQL'; }
  pre.src-sqlite:before { content: 'SQLite'; }
  /* additional languages in org.el's org-babel-load-languages alist */
  pre.src-forth:before { content: 'Forth'; }
  pre.src-io:before { content: 'IO'; }
  pre.src-J:before { content: 'J'; }
  pre.src-makefile:before { content: 'Makefile'; }
  pre.src-maxima:before { content: 'Maxima'; }
  pre.src-perl:before { content: 'Perl'; }
  pre.src-picolisp:before { content: 'Pico Lisp'; }
  pre.src-scala:before { content: 'Scala'; }
  pre.src-shell:before { content: 'Shell Script'; }
  pre.src-ebnf2ps:before { content: 'ebfn2ps'; }
  /* additional language identifiers per "defun org-babel-execute"
       in ob-*.el */
  pre.src-cpp:before  { content: 'C++'; }
  pre.src-abc:before  { content: 'ABC'; }
  pre.src-coq:before  { content: 'Coq'; }
  pre.src-groovy:before  { content: 'Groovy'; }
  /* additional language identifiers from org-babel-shell-names in
     ob-shell.el: ob-shell is the only babel language using a lambda to put
     the execution function name together. */
  pre.src-bash:before  { content: 'bash'; }
  pre.src-csh:before  { content: 'csh'; }
  pre.src-ash:before  { content: 'ash'; }
  pre.src-dash:before  { content: 'dash'; }
  pre.src-ksh:before  { content: 'ksh'; }
  pre.src-mksh:before  { content: 'mksh'; }
  pre.src-posh:before  { content: 'posh'; }
  /* Additional Emacs modes also supported by the LaTeX listings package */
  pre.src-ada:before { content: 'Ada'; }
  pre.src-asm:before { content: 'Assembler'; }
  pre.src-caml:before { content: 'Caml'; }
  pre.src-delphi:before { content: 'Delphi'; }
  pre.src-html:before { content: 'HTML'; }
  pre.src-idl:before { content: 'IDL'; }
  pre.src-mercury:before { content: 'Mercury'; }
  pre.src-metapost:before { content: 'MetaPost'; }
  pre.src-modula-2:before { content: 'Modula-2'; }
  pre.src-pascal:before { content: 'Pascal'; }
  pre.src-ps:before { content: 'PostScript'; }
  pre.src-prolog:before { content: 'Prolog'; }
  pre.src-simula:before { content: 'Simula'; }
  pre.src-tcl:before { content: 'tcl'; }
  pre.src-tex:before { content: 'TeX'; }
  pre.src-plain-tex:before { content: 'Plain TeX'; }
  pre.src-verilog:before { content: 'Verilog'; }
  pre.src-vhdl:before { content: 'VHDL'; }
  pre.src-xml:before { content: 'XML'; }
  pre.src-nxml:before { content: 'XML'; }
  /* add a generic configuration mode; LaTeX export needs an additional
     (add-to-list 'org-latex-listings-langs '(conf " ")) in .emacs */
  pre.src-conf:before { content: 'Configuration File'; }

  table { border-collapse:collapse; }
  caption.t-above { caption-side: top; }
  caption.t-bottom { caption-side: bottom; }
  td, th { vertical-align:top;  }
  th.org-right  { text-align: center;  }
  th.org-left   { text-align: center;   }
  th.org-center { text-align: center; }
  td.org-right  { text-align: right;  }
  td.org-left   { text-align: left;   }
  td.org-center { text-align: center; }
  dt { font-weight: bold; }
  .footpara { display: inline; }
  .footdef  { margin-bottom: 1em; }
  .figure { padding: 1em; }
  .figure p { text-align: center; }
  .inlinetask {
    padding: 10px;
    border: 2px solid gray;
    margin: 10px;
    background: #ffffcc;
  }
  #org-div-home-and-up
   { text-align: right; font-size: 70%; white-space: nowrap; }
  textarea { overflow-x: auto; }
  .linenr { font-size: smaller }
  .code-highlighted { background-color: #ffff00; }
  .org-info-js_info-navigation { border-style: none; }
  #org-info-js_console-label
    { font-size: 10px; font-weight: bold; white-space: nowrap; }
  .org-info-js_search-highlight
    { background-color: #ffff00; color: #000000; font-weight: bold; }
  .org-svg { width: 90%; }
  /*]]>*/-->
</style>
<script type="text/javascript">
/*
@licstart  The following is the entire license notice for the
JavaScript code in this tag.

Copyright (C) 2012-2019 Free Software Foundation, Inc.

The JavaScript code in this tag is free software: you can
redistribute it and/or modify it under the terms of the GNU
General Public License (GNU GPL) as published by the Free Software
Foundation, either version 3 of the License, or (at your option)
any later version.  The code is distributed WITHOUT ANY WARRANTY;
without even the implied warranty of MERCHANTABILITY or FITNESS
FOR A PARTICULAR PURPOSE.  See the GNU GPL for more details.

As additional permission under GNU GPL version 3 section 7, you
may distribute non-source (e.g., minimized or compacted) forms of
that code without the copy of the GNU GPL normally required by
section 4, provided you include this license notice and a URL
through which recipients can access the Corresponding Source.


@licend  The above is the entire license notice
for the JavaScript code in this tag.
*/
<!--/*--><![CDATA[/*><!--*/
 function CodeHighlightOn(elem, id)
 {
   var target = document.getElementById(id);
   if(null != target) {
     elem.cacheClassElem = elem.className;
     elem.cacheClassTarget = target.className;
     target.className = "code-highlighted";
     elem.className   = "code-highlighted";
   }
 }
 function CodeHighlightOff(elem, id)
 {
   var target = document.getElementById(id);
   if(elem.cacheClassElem)
     elem.className = elem.cacheClassElem;
   if(elem.cacheClassTarget)
     target.className = elem.cacheClassTarget;
 }
/*]]>*///-->
</script>
</head>
<body>
<div id="content">
<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#orgd84c8b4">1. Conexão com banco de dados</a>
<ul>
<li><a href="#org2a054c9">1.1. Abrindo a conexão</a></li>
<li><a href="#orgb67378d">1.2. Fechar a conexão</a></li>
<li><a href="#orga20d9b6">1.3. Exercício 1</a></li>
<li><a href="#org5f9cc51">1.4. Criando banco de dados MySQL</a></li>
<li><a href="#org41efd24">1.5. Exercício 2</a></li>
<li><a href="#org750f6e7">1.6. Criando tabelas</a></li>
<li><a href="#org89a499e">1.7. Exercício 3</a></li>
<li><a href="#org54c82ed">1.8. Inserindo dados</a></li>
<li><a href="#orgf7ee331">1.9. Exercício 4</a></li>
<li><a href="#org58742d1">1.10. Valores dinâmicos</a></li>
<li><a href="#org949944c">1.11. Exercício 5</a></li>
</ul>
</li>
</ul>
</div>
</div>
<div id="outline-container-orgd84c8b4" class="outline-2">
<h2 id="orgd84c8b4"><span class="section-number-2">1</span> Conexão com banco de dados</h2>
<div class="outline-text-2" id="text-1">
<p>
PHP possui três formas de trabalhar com MySQL:
</p>

<ul class="org-ul">
<li>MySQLi (orientado à objeto)</li>
<li>MySQLi (procedural)</li>
<li>PDO</li>
</ul>

<p>
PDO trabalha com 12 sistemas de banco de dados diferentes.
</p>

<p>
MySQLi trabalha apenas com banco de dados MySQL.
</p>
</div>

<div id="outline-container-org2a054c9" class="outline-3">
<h3 id="org2a054c9"><span class="section-number-3">1.1</span> Abrindo a conexão</h3>
<div class="outline-text-3" id="text-1-1">
<p>
Antes de acessar os dados em um banco de dados MySQL, você precisa se conectar ao servidor:
</p>

<pre class="example">
&lt;?php

$servidor = "localhost";
$usuario = "root";
$senha = "toor";

// Cria a conexão:
$conexao = mysqli_connect($servidor, $usuario, $senha);

// Verifica a conexão
if( $conexao == false ) {
   die("A conexão falhou: " . mysqli_connect_error());
}

echo "Conexão realizada com sucesso!";
?&gt;
</pre>
</div>
</div>

<div id="outline-container-orgb67378d" class="outline-3">
<h3 id="orgb67378d"><span class="section-number-3">1.2</span> Fechar a conexão</h3>
<div class="outline-text-3" id="text-1-2">
<p>
Quando o script termina a conexão com o banco de dados é fechada automaticamente. Mas podemos fechá-la antes:
</p>

<pre class="example">
mysqli_close($conexao);
</pre>
</div>
</div>

<div id="outline-container-orga20d9b6" class="outline-3">
<h3 id="orga20d9b6"><span class="section-number-3">1.3</span> Exercício 1</h3>
<div class="outline-text-3" id="text-1-3">
<p>
Crie uma página php chamada (teste.php) que verifica se a conexão com o servidor de banco de dados está sendo feita corretamente.
</p>
</div>
</div>

<div id="outline-container-org5f9cc51" class="outline-3">
<h3 id="org5f9cc51"><span class="section-number-3">1.4</span> Criando banco de dados MySQL</h3>
<div class="outline-text-3" id="text-1-4">
<p>
Um banco de dados é composto de várias tabelas.
</p>

<p>
Para criar o banco em PHP você efetua uma consulta (query) com o comando de criação:
</p>

<pre class="example">
mysqli_query($conexao, "CREATE DATABASE banco");
</pre>

<p>
A página completa deve:
</p>

<ul class="org-ul">
<li>criar a conexão com o servidor de banco de dados</li>
<li>efetuar a consulta</li>
<li>fechar a conexão</li>
</ul>

<pre class="example">
&lt;?php

$servidor = "localhost";
$usuario = "root";
$senha = "toor";

// Cria a conexão:
$conexao = mysqli_connect($servidor, $usuario, $senha);

// Verifica a conexão
if( $conexao == false ) {
   die("A conexão falhou: " . mysqli_connect_error());
}

echo "Conexão realizada com sucesso!&lt;br&gt;";

// Cria o banco de dados
$sql = "CREATE DATABASE bdEscola";
if (mysqli_query($conexao, $sql)) {
    echo "Banco de dados criado com sucesso!&lt;br&gt;";
} else {
    echo "Erro na criação do banco de dados: " . mysqli_error($conexao);
}

mysqli_close($conexao);
?&gt;
</pre>
</div>
</div>

<div id="outline-container-org41efd24" class="outline-3">
<h3 id="org41efd24"><span class="section-number-3">1.5</span> Exercício 2</h3>
<div class="outline-text-3" id="text-1-5">
<p>
Escreva uma página em php (cria.php) que cria um banco de dados chamado: bdLoja.
</p>
</div>
</div>

<div id="outline-container-org750f6e7" class="outline-3">
<h3 id="org750f6e7"><span class="section-number-3">1.6</span> Criando tabelas</h3>
<div class="outline-text-3" id="text-1-6">
<p>
Uma tabela de banco de dados possui dados dispostos em linhas e colunas.
</p>

<p>
O comando <b>CREATE TABLE</b> é usado para criar uma tabela em MySQL.
</p>

<p>
O comando abaixo cria uma tabela <b>alunos</b> com 3 colunas: id, nome, nota:
</p>

<pre class="example">
CREATE TABLE alunos (
   id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY,
   nome VARCHAR(40) NOT NULL,
   nota VARCHAR(5)
)
</pre>

<p>
A tabela poderia armazenar os seguintes dados:
</p>

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-left" />

<col  class="org-right" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-right">id</th>
<th scope="col" class="org-left">nome</th>
<th scope="col" class="org-right">nota</th>
</tr>
</thead>
<tbody>
<tr>
<td class="org-right">1</td>
<td class="org-left">Fulano</td>
<td class="org-right">5.50</td>
</tr>

<tr>
<td class="org-right">2</td>
<td class="org-left">Ciclano</td>
<td class="org-right">7.50</td>
</tr>

<tr>
<td class="org-right">3</td>
<td class="org-left">Beltrano</td>
<td class="org-right">10.00</td>
</tr>
</tbody>
</table>

<p>
O campo id "id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY" armazenará valores inteiros, começando em 1, os valores não serão fornecidos, o próximo valor será gerado automaticamente (AUTO_INCREMENT).
</p>

<p>
O campo nome "nome VARCHAR(40) NOT NULL" poderá armazenar strings de até 40 caracteres, é obrigatório fornecer um valor para este campo (NOT NULL).
</p>

<p>
O campo nota "nota VARCHAR(5)" poderá armazenar strings de até 5 caracteres, como ele guardará notas, os valores serão armazenados de 0.00 até 10.00.
</p>

<p>
A página que cria a tabela é parecida com a que cria banco de dados, mas agora devemos fornecer o banco no momento da criação da conexão. Assim a tabela é criada no banco fornecido.
</p>

<pre class="example">
&lt;?php

$servidor = "localhost";
$usuario = "root";
$senha = "toor";
$banco = "bdEscola"; // novo campo

// Cria a conexão:
$conexao = mysqli_connect($servidor, $usuario, $senha, $banco);

// Verifica a conexão
if( $conexao == false ) {
   die("A conexão falhou: " . mysqli_connect_error());
}

echo "Conexão realizada com sucesso!&lt;br&gt;";

// Cria a tabela
$sql = "CREATE TABLE alunos (
   id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY,
   nome VARCHAR(40) NOT NULL,
   nota VARCHAR(5)
)";

if (mysqli_query($conexao, $sql)) {
    echo "Tabela criada com sucesso!&lt;br&gt;";
} else {
    echo "Erro na criação da tabela: " . mysqli_error($conexao);
}

mysqli_close($conexao);
?&gt;
</pre>
</div>
</div>

<div id="outline-container-org89a499e" class="outline-3">
<h3 id="org89a499e"><span class="section-number-3">1.7</span> Exercício 3</h3>
<div class="outline-text-3" id="text-1-7">
<p>
Escreva uma página php que cria a tabela <b>clientes</b> no banco <b>bdLoja</b>. A tabela deve poder armazenar os dados:
</p>

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-left" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-right">id</th>
<th scope="col" class="org-left">nome</th>
<th scope="col" class="org-right">telefone</th>
<th scope="col" class="org-right">saldo</th>
</tr>
</thead>
<tbody>
<tr>
<td class="org-right">1</td>
<td class="org-left">Fulana</td>
<td class="org-right">3412039182</td>
<td class="org-right">0.00</td>
</tr>

<tr>
<td class="org-right">2</td>
<td class="org-left">Beltrano</td>
<td class="org-right">6709813112</td>
<td class="org-right">-5.00</td>
</tr>

<tr>
<td class="org-right">3</td>
<td class="org-left">Ciclano</td>
<td class="org-right">1790129832</td>
<td class="org-right">-99999.99</td>
</tr>
</tbody>
</table>
</div>
</div>

<div id="outline-container-org54c82ed" class="outline-3">
<h3 id="org54c82ed"><span class="section-number-3">1.8</span> Inserindo dados</h3>
<div class="outline-text-3" id="text-1-8">
<p>
Depois de criar o banco e a tabela podemos adicionar dados.
</p>

<p>
As regras são:
</p>

<ul class="org-ul">
<li>A consulta SQL deve ser escrita entre aspas.</li>
<li>Os valores que são string dentro da consulta devem aparecer entre apóstrofos</li>
<li>Valores numéricos não devem ser colocados em apóstrofos</li>
<li>A palavra NULL não deve ser colocada entre apóstrofos</li>
</ul>

<p>
O comando abaixo é usado para inserir dados:
</p>

<pre class="example">
INSERT INTO nome_tabela (coluna1, coluna2, coluna3,...)
VALUES (valor1, valor2, valor3,...)
</pre>

<p>
Para inserir dados na tabela <b>alunos</b> temos o comando:
</p>

<pre class="example">
INSERT INTO alunos (nome, nota) VALUES ('Fulano', '5.5')
</pre>

<p>
Note que a nota aparece entre apóstrofos (') porque é armazenada em um campo com tipo VARCHAR.
</p>

<p>
Novamente a página de inserção de dados é bem parecida com a página de criação de tabela.
</p>

<pre class="example">
&lt;?php

$servidor = "localhost";
$usuario = "root";
$senha = "toor";
$banco = "bdEscola"; 

// Cria a conexão:
$conexao = mysqli_connect($servidor, $usuario, $senha, $banco);

// Verifica a conexão
if( $conexao == false ) {
   die("A conexão falhou: " . mysqli_connect_error());
}

echo "Conexão realizada com sucesso!&lt;br&gt;";

// Insere uma linha na tabela
$sql = "INSERT INTO alunos (nome, nota) 
VALUES ('Fulano', '5.5')";

if (mysqli_query($conexao, $sql)) {
    echo "Registro criado com sucesso!&lt;br&gt;";
} else {
    echo "Erro na criação do registro: " . mysqli_error($conexao);
}

mysqli_close($conexao);
?&gt;
</pre>
</div>
</div>

<div id="outline-container-orgf7ee331" class="outline-3">
<h3 id="orgf7ee331"><span class="section-number-3">1.9</span> Exercício 4</h3>
<div class="outline-text-3" id="text-1-9">
<p>
Crie uma página que insere os seguintes clientes na tabela <b>clientes</b> criada no exercício anterior:
</p>

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">nome</th>
<th scope="col" class="org-right">telefone</th>
<th scope="col" class="org-right">saldo</th>
</tr>
</thead>
<tbody>
<tr>
<td class="org-left">Bisonho</td>
<td class="org-right">3499999999</td>
<td class="org-right">1.99</td>
</tr>

<tr>
<td class="org-left">Bela</td>
<td class="org-right">6788888888</td>
<td class="org-right">3.98</td>
</tr>

<tr>
<td class="org-left">Guru</td>
<td class="org-right">1766666666</td>
<td class="org-right">-5.97</td>
</tr>
</tbody>
</table>

<p>
Os valores de id não são fornecidos, mas gerados automaticamente.
</p>
</div>
</div>

<div id="outline-container-org58742d1" class="outline-3">
<h3 id="org58742d1"><span class="section-number-3">1.10</span> Valores dinâmicos</h3>
<div class="outline-text-3" id="text-1-10">
<p>
O comando abaixo possui os valores estáticos:
</p>

<pre class="example">
INSERT INTO alunos (nome, nota) VALUES ('Fulano', '5.5')
</pre>

<p>
Toda vez que o comando for executado o mesmo nome e nota será registrado. É possível receber valores do usuário e registrá-los:
</p>

<p>
A página abaixo recebe um nome e uma nota digitado pelo usuário e envia os dados para a página recebe.php
</p>

<pre class="example">
&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;
&lt;head&gt;
    &lt;meta charset="UTF-8"&gt;
    &lt;title&gt;Formulário&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
    &lt;form action="recebe.php"&gt;
        &lt;input type="text" name="nome"&gt;
        &lt;input type="text" name="nota"&gt;
        &lt;input type="submit" value="Enviar"&gt;
    &lt;/form&gt;
&lt;/body&gt;
&lt;/html&gt;
</pre>

<p>
A página recebe.php pode salvar o nome e a nota com SQL:
</p>

<pre class="example">
&lt;?php
$nomeDigitado = $_GET['nome'];
$notaDigitada = $_GET['nota];

$servidor = "localhost";
$usuario = "root";
$senha = "toor";
$banco = "bdEscola"; 

// Cria a conexão:
$conexao = mysqli_connect($servidor, $usuario, $senha, $banco);

// Verifica a conexão
if( $conexao == false ) {
   die("A conexão falhou: " . mysqli_connect_error());
}

echo "Conexão realizada com sucesso!&lt;br&gt;";

// Insere valores na tabela
$sql = "INSERT INTO alunos (nome, nota) 
VALUES ('$nomeDigitado', '$notaDigitada')";

if (mysqli_query($conexao, $sql)) {
    echo "Registro criado com sucesso!&lt;br&gt;";
} else {
    echo "Erro na criação do registro: " . mysqli_error($conexao);
}

mysqli_close($conexao);
?&gt;
</pre>
</div>
</div>

<div id="outline-container-org949944c" class="outline-3">
<h3 id="org949944c"><span class="section-number-3">1.11</span> Exercício 5</h3>
<div class="outline-text-3" id="text-1-11">
<p>
Usando php crie uma página (entrada.php) que recebe o nome de um cliente, o telefone e o saldo e envia para outra página criada por você (salva.php), que salva o cliente na tabela <b>clientes</b>.
</p>
</div>
</div>
</div>
</div>
<div id="postamble" class="status">
<p class="date">Created: 2019-09-23 seg 21:07</p>
<p class="validation"><a href="http://validator.w3.org/check?uri=referer">Validate</a></p>
</div>
</body>
</html>
