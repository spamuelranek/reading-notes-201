# STORAGE
### by Local

##[The Past, Present, and Future of Local Storage for Web Applications](http://diveinto.html5doctor.com/storage.html)
- The Past
  - Native applications benefit from persistent local storage
  - Cookies exist but can slow dow, be unsecure, and not do much
  - What we really want:
    - lot of storage space
    - on the client
    - persistent
    - isn't transmitted to server
- Brief overview of Past
  - several attempts and patch work of options were created to store information on client side for each page
- HTML 5
  - HTML Storage
    - creates key/value pairs that do persist
  - Using HTML
    - works on key/value pairs
    - the key is a string
      - it can be other things but it must be coerced into a string
  - Current Limitations
    - 5MB is what is alloted in first creation
    - `QUOTA_EXCEEDED_ERR` if you exceed the 5MB allotment
```js
//diveinto.html
function saveGameState(){
    if (!supportsLocalStorage()) {return false;}
    localStorage["halma.game.in.progress"] = gGameInProgress;
    for (var i = 0. i<kNumPieces; i++){
        localStorage["halma.piece. " + i + ".row"] = gPieces[i].row
        localStorage["halma.piece. " + i + ".row"] = gPieces[i].column;
    }
    localStorage['halma.selectedpiece'] = gSelectedPieceIndex;
    localStorage['halma.selectedpiecehasmoved'] = gSelectedPieceHasMoced;
    localStorage['halma.movecount'] = gMoveCount;
    return true;
}
```
- that is to store the information

```js
//diveinto.html
function resumeGame(){
    if (!supportsLocalStorage()) {return false;}
    gGameInProgress = (localStorage['halma.game.in.progress'] == 'true');
    if(!GameInProgress){return false;}
    gPieces = new Array(kNumPieces);
    for (var i = 0; i <kNumPieces; i++)
        var row = parseInt(localStorage['halma.piece.' + i + '.row']);
        var column = parseInt(localStorage['halma.piece.' + i + '.column']);
        gPieces[i] = new Cell(row,column);
    }
    gNumPieces = kNumPieces;
    gSelectedPieceIndex = parseInt(localStorage['halma.selectedpiece']);
    gSelectedPieceHasMoved = localStorage['halma.selectedpiecehasmoved'] == "true";
    gMoveCount = parseInt(localStorage['halma.movecount']);
    drawBoard();
    return true;
}
```
- this is to retrieve the stored data
  - but again remember the data is return as a string and must be treated as such

- this paper was written in 2011 and HTML 5 has become a standard
  - I wonder what the norm for local storage has become