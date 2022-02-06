## My Logical Thinking Course - Notes :books:



###### Herbrand Semantics

Object constants, function constants and relation constants of our language;

Herbrand base: The set of all ground atoms that can be formed form theses components;

Not compact;

Deficiency: There are restrictions on the cardinality of the worlds that can be axiomatized;

###### Tarskian Semantics

Will not be used;



_LPL_ Language, proof, and Logic;



**Lecture (Optional): Stanford CS 157 2021 - Lecture 1**

Uses of logic:

Theorems in Mathematics, hardware engineering, configuration of gates,  circuits, software engineering, debugging programs, rules and regulations, rules for a game, communication;



> Logic is the mathematics of the computer science as Calculus is the mathematics of physics;<



Elements of Logic:

Ex: Friends. Some like each other, some don't.

We usually have tips of information, about who likes who...we might get or figure out, by what others say.

We take theses little bits of information and figure out what we can conclude of that info, that's what logic does.

tidbits;

Given the premises, something are really not true, and some, we don't know.



Model checking;

Enumerating all the possibilities; It may not work, if you have thousand of possibilities;

Symbolic manipulation: Conclusions based on the sentences, form of them, with the structure of the sentence, not with the meaning. 

"" All x are Y

All y are z

Therefore, all x are z. ""



Inference doesn't work;

Sound if rules of inference is called deduction;

Incomplete induction: From the specific to general

**Induction** is not necessarily sound (but it can be useful)

Deduction is necessarily sound.



**Induction** is the basis for Science (and machine learning);

Form general theory about the world when we look at it, but sometimes is wrong.

Deduction is the subject matter of Logic;



Science aspires to discover new knowledge

Logic aspires to derive conclusions **implied** by premises.



Deduction and induction are complementary;

*"You are not thinking; You are just being logical"* Stein



### **Elements of Logic**:

**Logical Language** - Definitions: A triangle is a polygon with 3 sides

Constraints: Parents are older than their children

Partial Info: Abby likes one of Cody or Dana.



**Logical Reasoning** 

Model Checking - Truth Tables, Logic Grids

Equivalence Transformations - Symbolic Manipulation Proofs



**"Metalevel" Concepts and Analysis**

Validity, Contingency, Unsatisfiability

Equivalence, Entailment, Consistency

Soundness, Completeness, Decidability



Aplicamos a lógica, por exemplo, nos sistemas de computador, com os leitores de e-mails, eles podem escrever regras para gerenciar mensagens que chegam - deletando algumas, movendo outras para diferentes caixas de entrada, e assim vai...baseados nas propriedades daquelas mensagens; No sistema comercial, eCommerce system, permmite que as empresas possam estabelecer um preço, baseado no produto, cliente, data, e assim vai...



**Possible Worlds**

Por exemplo, um grupo de 4 garotas, que podem gostar ou não uma da outra;

Um grupo de 16 possibilidades 4x4; Elevado a 2 opções: verdadeiras ou falsas;

Então...2 possibilidades de verdadeiro e falso com 16 outras possibilidades: 2 elevado a 16: 65.536 possibilidades; Como não sabemos o que elas pensam, temos pessoas que nos contam;

Cada uma pode dizer em uma sentença lógica, o que sabe; Colhemos essas partes de informações pra chegar a conclusões, e podemos usar provas lógicas para explicar nossas conclusões para outros;

**Logical Sentences**

> Uma comunicação efetiva, exige uma linguagem que nos permita expressar o que sabemos, nemmais nem menos. Apenas o que sabemos. "A beleza da Lógica, é que ela nos dá os meios de expressar informação incompleta quando isso é tudo que temos, e expressar informação completa quando a informação completa está disponível"



**Logical Entailment**

Uma maneira de checar quando as sentenças vinculam com uma conclusão é examinar todos os worlds onde a sentença dada é verdadeira;

Por exemplo, no set de 4 cards, com possibilidades, você examina, nos 4 cards eu tenho a mesma informação como verdadeira? Ou em apenas um deles? Ou melhor, essa informação varia em outros cards? Pode ser verdadeira em um e falsa no outro?... Então, chegar a a uma conclusão de true/false ainda não seria possível porque ainda não temos aquele conhecimento.

**Logical Proofs**

Mas fazer essa checagem de possible worlds não é muito prático, em geral.

A alternativa é *logical reasoning* a saber aplicação de regras de raciocínio pra derivar conclusões lógicas e produzir *logical proofs*. Premissas à conclusões.

> We need to be familiar with the reasoning atoms, out of which complex proof "molecules" are built.

 

O que distingue um padrão correto de um falso é que ele semrpre tem que conduzir a conclusões corretas. Eles tem que ser corretos baseados nas premissas em que foram baseados.



**Automation**

We use the formal representation to encode the premisses of a problem as data structures in a computer, and we programm the computer to encode the premisses of a problem as a data structure ina computer, and we program the computer to apply the rules in a systematic way. The rules are appplied until the desired conclusion is attained or until it is determined that the desired conclusion cannot be attained.

*Boole gave substance to this dream in the 1800s with the invention of Boolean algebra and with the creation of a machine capable of computing accordingly.*

 Today, the prospect of automated reasoning has moved from the realm of possibility to that of practicality, with the creation of *logic technology* in the form of automated reasoning systems, such as Vampire, Prover9, the Prolog Technology Theorem Prover, Epilog, and others.

*Logical Spreadsheets.* Logical spreadsheets generalize traditional spreadsheets to include logical constraints as well as traditional arithmetic formulas. Examples of such constraints abound. For example, in scheduling applications, we might have timing constraints or restrictions on who can reserve which rooms. In the domain of travel reservations, we might have constraints on adults and infants. In academic program sheets, we might have constraints on how many courses of varying types that students must take.

##### Propositional Logic

 Roughly speaking, a *proposition* is a possible condition of the world that is either true or false, e.g. the possibility that it is raining, the possibility that it is cloudy, and so forth

1. Simple sentences (propositional constants/logical constants): simple facts about the world
2. Compund Sentences: Logical relationships between the simpler sentences pf which they are composed.

Types of compound sentences:

*Negation* negation operator and an arbitrary sentence, called the target. Eg. (¬p)

*Conjunction* sequência de ocorrências separadas por ocorrências do operador ^ entre parênteses eg. (p ^ q)

*Disjunction* sequência de frases separadas por ocorrências do operador v, entre parênteses. eg. (p v q)

*Implication* par de frases separadas pelo operador (flecha para direita) entre parênteses. A sentença da esquerda é chamada de antecedente, e a da direita consequente. 

*Biconditional* Combinação de implicação e uma implicação reversa. (Flecha bidirecional)



> Os operadores tem níveis de prioridade, assim como multiplicaçã na matemática sempre vem antes da soma. O operador ¬ é maior que ^; ^ é maior que v; v é maior que (flecha pra direita); (flecha pra direita) é maior que (flecha bidirecional); Isso falando na questão de prioridade, caso vários operadores estejam em uma mesma linha e sem parênteses.



Exemplos: 

| ¬ *p* ∧ *q*     | ((¬ *p*) ∧ *q*)      |
| --------------- | -------------------- |
| *p* ∧ ¬*q*      | (*p* ∧ (¬ *q*))      |
| *p* ∧ *q* ∨ *r* | ((*p* ∧ *q*) ∨ *r*)  |
| *p* ∨ *q* ∧ *r* | (*p* ∨ (*q* ∧ *r*))  |
| *p* ⇒ *q* ⇔ *r* | ((*p* ⇒ *q*) ⇔ *r*)) |
| *p* ⇔ *q* ⇒ *r* | (*p* ⇔ (*q* ⇒ *r*))  |



*"When an operand is surrounded by two ∧ operators or by two ∨ operators, the operand associates to the left. When an operand is surrounded by two ⇒ operators or by two ⇔ operators, the operand associates to the right."*



##### Semântica

A *truth assignment* for a propositional vocabulary is a function assigning a truth value to each of the proposition constants of the vocabulary. In what follows, we use the digit 1 as a synonym for *true* and 0 as a synonym for *false*; and we refer to the value of a constant or expression under a truth assignment *i* by superscripting the constant or expression with *i* as the superscript.

##### Avaliação

Substituimos valores verdadeiros e falsos pelas constantes de proposição nas frases, formando uma expressão com 1s e 0s e com operadores lógicos.

Nós usamos operadores semânticos para avaliar sub expressões com aqueles argumentos verdadeiros. Depois repetimos, até termos uma frase verdadeira por completo.
