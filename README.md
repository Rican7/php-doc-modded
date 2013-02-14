# PHP-Doc-Modded

The original plugin (information below) was **wonderful**.. unfortunately it has some issues but is no longer supported by the original developer.

Here's my modified version. :kthxbye:


Below is the original README information from http://www.vim.org/scripts/script.php?script_id=1355
------------------- 

PDV (phpDocumentor for Vim) 
======================== 

Version: 1.0.0 

Copyright 2005 by Tobias Schlitt <toby@php.net> 
Inspired by phpDoc script for Vim by Vidyut Luther (http://www.phpcult.com/). 

Provided under the GPL (http://www.gnu.org/copyleft/gpl.html). 

This script provides functions to generate phpDocumentor conform 
documentation blocks for your PHP code. The script currently 
documents: 

- Classes 
- Methods/Functions 
- Attributes 

All of those supporting all PHP 4 and 5 syntax elements. 

Beside that it allows you to define default values for phpDocumentor tags 
like @version (I use $id$ here), @author, @license and so on. 

For function/method parameters and attributes, the script tries to guess the 
type as good as possible from PHP5 type hints or default values (array, bool, 
int, string...). 

You can use this script by mapping the function PhpDoc() to any 
key combination. Hit this on the line where the element to document 
resides and the doc block will be created directly above that line. 

Changelog 
========= 

Version 1.0.0 
------------------- 

* Created the initial version of this script while playing around with VIM 
scripting the first time and trying to fix Vidyut's solution, which 
resulted in a complete rewrite.

install details
Installation 
========= 

For example include into your .vimrc: 

	source ~/.vim/php-doc.vim 
	inoremap <C-P> <ESC>:call PhpDocSingle()<CR>i 
	nnoremap <C-P> :call PhpDocSingle()<CR> 
	vnoremap <C-P> :call PhpDocRange()<CR> 

This includes the script and maps the combination <ctrl>+p 
to the doc functions.
