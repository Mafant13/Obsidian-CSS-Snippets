/* pseudo(meta) spoiler tags */ 
/* blacks out non-hovered-nonactive text surrounded in *~~text~~* */
.theme-light{
  --spoiler-bg: #111;
}

.theme-dark{
  --spoiler-bg: #EEE;
}

div:not(.CodeMirror-activeline) > .CodeMirror-line .cm-em.cm-strikethrough,
em > del {
font-style: initial;
text-decoration: unset;
background-color: var(--spoiler-bg);
color: var(--spoiler-bg);
}

.CodeMirror-activeline > .CodeMirror-line .cm-em.cm-strikethrough,
em > del:hover,
.cm-em.cm-strikethrough:hover {
background-color: var(--background-secondary-alt) !important;
}
