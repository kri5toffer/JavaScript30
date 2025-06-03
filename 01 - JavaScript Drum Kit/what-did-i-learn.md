- each key has a data-key number 
- when a key is pressed, the keydown event is triggered
- document.querySelector finds the first element that matches the selector

- audio[data-key="${e.keyCode}"]`
    - e is the event object that holds the key code
    - audio selects all <audio> elements
    - [data-key="${e.keyCode}"] selects the audio element that has the same data-key as the key code

- calling a audio file on top of another audio file will not play the second time

- document.querySelector(`.key[data-key="${e.keyCode}"]`) s
    - .querySelector is a method that selects the first element that matches the selector
    - backticks allos you to insert variables into a string
    -.key selects elements with this class = "key"
    -[data-key="${e.keyCode}"] selects elements with data-key attributes equal to the value of e.keyCode
EG find: <div data-key="65" class="key">...</div>

-keys.forEach(key => key.addEventListener('transitionend', removeTransition));
    -transitionend is an event that is triggered when a transition ends


key.classList.add("playing")
- .classList is a property that lets you add and remove classes from an element
- .add() is a method that adds a class to an element
- "playing" is the class that we want to add to the key element


