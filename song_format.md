# Song Format

Songs content requires a **name**, a **key** and **content**. Name and Key should be self-explanatory. The content consists of lyrics and chords but is expected to be in a particular format detailed below.

Song content should be input using a monospaced font (fonts where all characters have the same width. `Courier New` is a fairly common font that has this characteristic.). Monospaced fonts give the user the ability to accurately place chords above the correct words/syllables in the lyrics. 

It should be fairly easy to find songs online already in this format or very close to it (it would require very minor editing to have the song match the format). 

Lines in the content should be of two types:

1. **Chord** lines: lines that contain ONLY chords
2. **Lyric** lines: lines that contain lyrics or an empty line (everything that is not a chord line is a lyric/text line).

## Chord lines
Chord lines consist only of **chords** separated by **spaces** (not tabs). Chords _begin_ with CBDEFGAB, optionally followed by an accidental # (sharp) or b (flat). It does not handle double sharps ## or double flats bb as they rarely show up and introduce extra complexity with transposition.

Chords may optionally have any of the following modifiers:

1. m (minor)
2. sus (suspended)
3. aug (augmented)
4. dim (diminished)
5. maj (major. using this notation is discouraged in favor of just leaving it out.)
6. min (minor. using the 'm' notation is preferred)

Chords and modifiers can also be followed by any single digit number: e.g. Asus2
And lastly you can have bass note notation by adding a slash '/' followed by a single note: e.g. E/G#

The following examples are valid chord notation:

1. G (G major)
2. Bm (B minor)
3. F#m7 (F sharp minor 7)
4. Asus2 (A suspended 2)
5. D/F# (D major F sharp bass)


Do NOT add anything to a chord line other than chords. The following is an invalid chord line:

```
G    C    D/F#     C    (repeat chorus)
```

It is invalid because "(repeat chorus)" is not a chord, and will be interpreted as a lyric line.

## Lyric lines
Lyric lines can contain any character and are meant to match up with chord lines. If a chord line is immediately followed by a lyric line, it is assumed that the two lines are a pair. 

If you would like to have a chord line be independent of any lyrics (e.g. for a intrumental interlude) let the line immediately following it be blank.

###The space and the underscore
There will be times when the lyric line will not have enough space to fit all the chords properly above. When this happens in-between words, use spaces to shift the lyric line. If this happens within a word, use an underscore.

Using underscores:
```
           Em7    Asus A   D
To look on him an par__don me
```
Using spaces:
```
E    A2 F#m B      E       A2 F#m B 
Your love     is extravagant
```
