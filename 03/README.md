# Chessboard

Write a program that creates a string that represents an 8x8 grid, using newline characters to seperate lines. At each position of the grid there is either a space or a "#" character. THe characters should from a chessboard.

## Algorigramme

![](algo.png)

## Pseudo-code

```
chessboard <- ''
Pour i de 1 jusqu'a 8 avec un pas de 1 :
    Pour j de 1 jusqu'a 8 avec un pas de 1 : 
        ajout chessboard <- '# '
    Fin Pour
    Si i % 2 :
        ajout '\n ' <- chessboard
    sinon :
        ajout chessboard <- '\n'
Fin Pour
```

## Code

```js
let chessboard = '';

for(let i = 0; i < 8; i++) {
    for(let j = 0; j < 8; j++) {
        chessboard += '# ';
    }
    chessboard += !(i % 2) ? '\n ' : '\n';
}
console.log(chessboard);

// Or

chessboard = '';
for(let i = 0; i < 8; i++) {
    chessboard += !(i % 2) ? ' # # # # # # # #\n' : '# # # # # # # #\n';
}
console.log(chessboard);

```
