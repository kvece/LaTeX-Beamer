# LaTeX Beamer Template

A set of commands and environments that establishes a base template for beamer

## Usage

Look at example.tex for a demo of the functionality

### Commands

`\setlogo{Picture.jpg}`
Set the logo for all the slides

`\slidetitle{Line 1}{Line 2}{Line 3}{Line 4}`
Make the title slide

`\classification{Value}`
Set the classification for the following slides

##### Classification Values

You can use any of the following:

| Classifications |
| ------------- |
| \unclassified |
| \confidential |
| \secret       |
| \topsecret    |
| ------------- |

Each one of these can also take an individual releasibility

###### Example
`\unclassified[//FOUO]`
Makes an Unclassified//FOUO tag for the slides

`\slidetransition{Transition}`
Use this slide to transition from one topic to another

`\slideprompt{Prompt}`
Use this slide to prompt the audience

`\slidepicture{Title}{Picture.jpg}`
Use this slide to make a picture with a title

`\slidefullpicture{Picture.jpg}`
Use this slide to make a full screen picture


### Environments
`slide`
Use this environment to start a new slide

###### Example

```
\begin{slide}{Title}
    My Text
\end{slide}
```

`slidepictureleft`
Use this environment to put a picture on the left of the slide

###### Example

```
\begin{slide}{Title}
    \begin{pictureleft}{Picture.jpg}
        \begin{itemize}
            \item Point 1
            \item Point 2
            \item Point 3
        \end{itemize}
    \end{pictureleft}
\end{slide}
```

`slidepictureright`
Use this environment to put a picture on the right of the slide

###### Example

```
\begin{slide}{Title}
    \begin{pictureright}{Picture.jpg}
        \begin{itemize}
            \item Point 1
            \item Point 2
            \item Point 3
        \end{itemize}
    \end{pictureright}
\end{slide}
```


