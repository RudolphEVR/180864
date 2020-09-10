# Instrucciones
1.	Programar en el lenguaje de programación asignado (F#, Perl, Rust)
2.	Los programas están ubicados en la carpeta (source_code). 
3.	El código se debe compilar en cualquier sistema operativo. 
4.	El código se sube en https://github.com/upslp-teoriacomputacional/matricula 
5.	Ejemplo. 00180864_conjuntos. go
6.	El programa se evaluará de acuerdo con la rúbrica que se anexa. 
7.	Las evidencias del programa desarrollado es la plantilla del código fuente comentado.
8.	También se puede mostrar el funcionamiento de los programas en los inicios o términos de clase antes de la fecha límite.


## Rubrica
---
Funcionalidad: El programa funciona correctamente y todas las variables de entrada están validadas.
Razonamiento lógico: Es un código compacto muy depurado.
Estructuración del código: Si utiliza sangría, espacios e interlineado que dé mayor claridad.
Documentación: La presentación incluye el nombre, los apellidos, la carrera, nombre del profesor especialidad, nombre de la institución y matrícula, objetivos bien definidos documentados y partes del código bien documentado.
tags: [ 'Programming' ]
---

<div id = "content">
   <H1>Writing Clear Code</H1>
<p><br>


The overarching goal when writing code is to make it
easy to read and to understand. Well-written programs
are easier to debug, easier to maintain, and have 
fewer errors.
Writing a program is a lot like writing an essay.
When writing an essay, your message is more convincing when it is
accompanied by proper grammar and punctuation. When writing computer programs,
you should follow the same principle. It is even more important when programming
since someone may be assigned to maintain and support your code for long
periods of time. You will appreciate the importance of good style when it is
your task to understand and maintain someone else's code!

<p><h2>Coding.</h2>

<ul>

<p><li> Keep programs and methods short and manageable.

<p><li> Use language-specific idioms.

<p><li> Use straightforward logic and flow-of-control.

<p><li> Avoid magic numbers (numbers other than &minus;1, 0, 1, and 2);
instead, give them meaningful symbolic names.

</ul>



<p>
<br>

<h2>Naming conventions.</h2>

Here are some general principles when choosing names for
your variables, methods, and classes.

<ul>
<p><li> Use meaningful names that convey the purpose of the variable.
Choose names that are easy to pronounce, and avoid cryptic abbreviations.
For example, use <tt>wagePerHour</tt> or <tt>hourlyWage</tt> instead of <tt>wph</tt>.
Use <tt>polygon</tt> instead of
<tt>p</tt> or <tt>pgon</tt>.

<p><li> Be consistent.

<p><li> Name <tt>boolean</tt> variables and methods so that their
meaning is unambiguous, e.g., <tt>isPrime</tt> or
<tt>isEmpty()</tt> or <tt>contains()</tt>.

<p><li> Use shorter names (e.g., <tt>i</tt>) for short-lived variables
and loop-index variables.
Use more descriptive names for variables that serve an important purpose.

<p><li> Avoid generic names like <tt>foo</tt> or <tt>tmp</tt>
and meaningless names like <tt>fred</tt>.
Use terminology from the application domain when possible.

<p><li> Name a constant by its meaning, not its value,
e.g., name your variable <tt>DAYS_PER_WEEK</tt> instead of <tt>SEVEN</tt>.

</ul>


<p>
<blockquote>
<table cellspacing="1" cellpadding="5" border="0" bgcolor = "#ffffff" width = 700>
<tr>
<th>IDENTIFIER</th>
<th>NAMING RULES</th>
<th>EXAMPLE</th>
</tr>


<tr bgcolor = "#ebebeb">
<td align = "center">Variables</td>
<td>
A short, but meaningful, name that communicates to the 
casual observer what the variable represents,
rather than how it is used.  
Begin with a lowercase letter and use camel case
(mixed case, starting with lower case).
</td>
<td>
<code>
mass<br>
hourlyWage<br>
isPrime
</td>
</tr>

<tr bgcolor = "#ebebeb">
<td align = "center">Constant</td>
<td>
Use all capital letters, separating internal words with
the underscore character.
</td>
<td>
<code>
BOLTZMANN<br>
MAX_HEIGHT
</td>
</tr>

<tr bgcolor = "#ebebeb">
<td width = 130 align = "center">Class</td>
<td width = 330>
A noun that communicates what the class represents.
Begin with an uppercase letter and use camel case for internal words.
</td>
<td width = 130>
<code>
Complex<br>
Charge<br>
PhoneNumber
</td>
</tr>


<tr bgcolor = "#ebebeb">
<td align = "center">Method</td>
<td>
A verb that communicates what the method does.
Begin with a lowercase letter and use camelCase for
internal words.
</td>
<td>
<code>
move()<br>
draw()<br>
enqueue()
</td>
</tr>

</tbody>
</table>
</blockquote>





<h2>Commenting.</h2>

Programmers use comments to annotate a program and help the reader (or grader)
understand how and why your program works.
As a general rule, the code explains to the computer and programmer
<em>what</em> is being done; the comments explain to the programmer
<em>why</em> it is being done.
Comments can appear anywhere within a program where whitespace is allowed.
The Java compiler ignores comments.

<ul>
<li><em>Line comments.</em>
An end-of-line comment begins with <tt>//</tt> (two forward slashes) and
ends at the end of the line on which the forward slashes appear.
Any text from the <tt>//</tt> to the end of the line is ignored.

<li><em>Block comments.</em>
A block comment begins with <tt>/*</tt> (a forward slash and asterisk)
and ends with <tt>*/</tt> (asterisk and a forward slash).
Any text between these delimiters (even if it spans multiple lines) is ignored.

<li><em>Bold comments.</em>
A bold comment is a special case of a block comment designed to draw
attention.

<blockquote>
<table>
<TR><TD><pre>
/*---------------------------------------------------------
 *  Here is a block comment that draws attention
 *  to itself.
 *---------------------------------------------------------*/
</pre></td></tr>
</table>
</blockquote>

<li><em>Programming Languages doc comments.</em>
A doc comment is a special case of a block comment that begins with
 <tt>/**</tt> 
(a forward slash and two asterisks).
They are typically used to automatically generate the API for a class. 
Here are guidelines for
<a href = "https://fsharp.org/learn/">
writing F# comments</a>.
</ul>

<a href = "https://perldoc.perl.org/perl.html">
writing Perl comments</a>.
</ul>

<a href = "https://www.rust-lang.org/learn">
writing Rust comments</a>.
</ul>


<p>
There is no widely agreed upon set of rules.
Good programmers write code that documents itself.



<ul>
<p><li> Make sure that comments agree with the code. Be careful to
update the comments when you update the code.

<p><li> Do not write comments that merely restate the code.
Generally, comments should describe <em>what</em>
or <em>why</em> you are doing something, rather than <em>how</em>.

<blockquote>
<table>
<TR><TD><pre>
i++;      //  increment i by one
</pre></td></tr>
</table>
</blockquote>

<p><li> Comment any potentially confusing code, or better yet, rewrite
the code so that it isn't confusing.



<p><li> Include a bold comment at the beginning of each 
file with your name and a description of the program.
Many programmers also like to put the date and instructions 
for executing it.

<blockquote>
<table>
<TR><TD><pre>
/* *****************************************************************************
 *  Name:    Alan Turing
 *  NetID:   aturing
 *  Precept: P00
 *
 *  Description:  Prints 'Hello, World' to the terminal window.
 *                By tradition, this is everyone's first program.
 *                Prof. Brian Kernighan initiated this tradition in 1974.
 *
 *  Written:       5/03/1997
 *  Last updated:  8/22/2018
 *
 *  % python 3 HelloWorld.python
 *  % pyton HelloWorld
 *  Hello, World
 *
 **************************************************************************** */
</pre></td></tr>
</table>
</blockquote>



<p><li> Comment every important variable name (including 
all instance variables).

<blockquote>
<table>
<TR><TD><pre>
private double rx, ry;    //  position
private double q;         //  charge
</pre></td></tr>
</table>
</blockquote>



<p><li> Comment each method with a description of what it does.
Include what it takes as input, what it returns as output, and any
side effects. Use the parameter variable names in your description.

<blockquote>
<table>
<TR><TD><pre>
/*
 * Rearranges the elements of the array a[] in uniformly random order.
 * Throws an IllegalArgumentException if a is null.
 */
public static void shuffle(String[] a)
</pre></td></tr>
</table>
</blockquote>

If you prefer, you may use
<a href = "https://en.wikipedia.org/wiki/Structured_programming">doc comments</a>.

</ul>




<h2>Whitespace.</h2>

Programmers use whitespace in their code to make it easier to read.

<ul>

<p><li> Don't put more than one statement on a line.

<p><li> Use blank lines to separate your code into logical sections.

<p><li> Put a space between all binary operators 
(e.g., <tt><=</tt>, <tt>=</tt>, <tt>+</tt>) and their operands.
<!--  <tt>.</tt> operator is a separator, not a binary operator  -->
One possible exception is to emphasize precedence.

<blockquote>
<table>
<TR><TD><pre>
a*x + b
</pre></td></tr>
</table>
</blockquote>

<p><li> Include a space between a keyword (e.g., <tt>while</tt>,
<tt>for</tt>, <tt>if</tt>) and its opening parenthesis.

<p><li> Put a space after each statement in a <tt>for</tt> loop.

<blockquote>
<table>
<TR><TD><pre>
for(int i=0;i&lt;n;i++)    vs.      for (int i = 0; i < n; i++)
</pre></td></tr>
</table>
</blockquote>

<p><li> Put a space after each comma in an argument list.

<p><li> Put space after each comment delimiter.

<blockquote>
<table>
<TR><TD><pre>
    //This comment has no space           //  This comment has two 
    //after the delimiter and is          //  spaces after the delimiter
    //difficult to read.                  //  and is easier to read.
</pre></td></tr>
</table>
</blockquote>

<p><li> Do not put spaces before a semicolon.

<p><li> Do not put spaces between an object name, the <tt>.</tt> separator,
and a method name.

<p><li> Do not put spaces between a method name and its left parenthesis.


<p><li> Include blank lines to improve readability by grouping
blocks of related code.

<p><li> Use spaces to align parallel code whenever it enhances readability.

<blockquote>
<table>
<TR><TD><pre>
int n      = Integer.parseInt(args[0]);      //  size of population
int trials = Integer.parseInt(args[1]);      //  number of trials
</pre></td></tr>
</table>
</blockquote>

</ul>



<h2>Indenting.</h2>
Programmers format and indent their code to reveal structure, much
like an outline.

<ul>

<p><li> Avoid lines longer than 80 characters.

<p><li> Do not put more than one statement on a line.

<p><li> Indent a fixed number of spaces. We recommend 4.

<p><li> Always use spaces instead of tabs.
Modern IDEs (including <em>IntelliJ</em>) insert spaces when you
type the tab key&mdash;these are known as <em>soft tabs</em>.
Hard tabs are obsolete: in ancient times, they were used for data compression.

<p><li> Use a new indentation level for every level of nesting in your program.

<p><li> Follow either the K&R or BSD/Allman
<a href = "http://en.wikipedia.org/wiki/Indent_style">indentation styles</a> for
curly braces, and use it consistently. We consistently 
use the former for the booksite and the latter in the textbook.


<blockquote>
<table>
<TR><TD><pre>
//  K&R style indenting                   
public static void  main(String[] args) {
    System.out.println("Hello, World");
}

//  BSD-Allman style indenting
public static void main(String[] args)
{
    System.out.println("Hello, World");
}
</pre></td></tr>
</table>
</blockquote>


</ul>


<h4>Q + A</h4>

<p><b>Q.</b> Are there any official coding standards?
<p><b>A.</b>
Here are <a href = "codeconventions-150003.pdf">Sun's Code Conventions for the Java Programming Language</a>.
However, this document was written in 1997 and is no longer being maintained.

<p><b>Q.</b> Any good references on programming style?
<p><b>A.</b> <a href = "http://www.cs.princeton.edu/~bwk/tpop.webpage">The Practice
of Programming</a> by Brian W. Kernighan and Rob Pike is a classic.

<p><b>Q.</b> Do Java comments nest?
<p><b>A.</b> No. So you cannot eliminate a block of code
by simply surrounding it with the block comment delimiters (since the
block itself may contain a <tt>*/</tt> delimiter).

<p><b>Q.</b> How can I autoindent my code?
<p><b>A.</b> Use an editor designed for writing code. For example, if you used our
Java installer, <em>IntelliJ</em>
will automatically indent and reformat your code when you save it.

<p><b>Q.</b> Are there tools for enforcing coding style?
<p><b>A.</b> Yes, we recommend <a href = "http://checkstyle.sourceforge.net/">Checkstyle</a>.
If you followed our Windows, Mac OS X, or Linux instructions, <em>IntelliJ</em> is configured
to run Checkstyle automatically while you are editing.

<p><b>Q.</b> How can I write unmaintainable code?
<p><b>A.</b> Here's one guide to designing
<a href = "http://mindprod.com/jgloss/unmain.html">unmaintainable code</a>
and here's <a href = "http://archive.is/Pn5hH">another</a>.



<H4>Exercises</H4>

<ol>

<li><b>Fun with comments.</b>
What is the value of <tt>a</tt> after the following code fragment is executed?
<blockquote>
<table>
<TR><TD><pre>
//*/
a = 17;
/*/
a = -17;
//*/
</pre></td></tr>
</table>
</blockquote>   
Repeat the question after deleting the first <tt>/</tt>.


<li><b>More fun with comments.</b>
What does the following print?
<blockquote>
<table>
<TR><TD><pre>
public static void main(String[] args) { 
   boolean nesting = true;
   /* /* */ nesting = false; // */ 
   System.out.println(nesting);
} 
</pre></td></tr>
</table>
</blockquote>   
<p><em>Answer</em>: this code prints <tt>true</tt> if <tt>/*</tt>
comments can nest and <tt>false</tt> if they can't. Since Java
comments don't nest, it prints <tt>false</tt>.

</ol>

<p></p>
Don't be afraid of email harvesting, write your email properly and the page will perform programming obfuscation.

<small> <a href="" target="\_blank">@</a> for this feature!</small>
