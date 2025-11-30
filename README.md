# Emergency-Preparedness
This game will test you on your decision-making in the face of disasters. Be wise in your choices to survive the disaster.

Project Title
- Emergency Preparedness: Test Your Choices during Disasters

Problem Statement
- You can't stop disasters from happening all around the world at any point of the day, but you can control how you respond to it. Those who are unaware of what to do during those times are more likely to face grave injuries and death.

Project Objectives
- Our program will help users understand what to do during different disasters of their choosing through an interactive game where they make choices based on the given scenario and disaster. This can help in spreading awareness and facts about disasters so that more peaople can have a better understanding on how every action can affect them during those times.

Planned Features
-  Our program will use loops, built-in commands, functions, etc. to make our game interactive and fun.

Planned Inputs and Outputs
- Firstly, the user will input their name, setting, and disaster, which are prompted by the pogram. The program will then return a scenario with the chosen disaster and setting and will ask the user to make a choice, depeding on the scenario. It will result in different endings depending on the choices the user made throughout the game.

Logic Plan:
Psuedocode:

start program

function main()
  display "Welcome to our game where we will test your ability to make the right decisions during disasters."
  display "Pick a disaster (enter 1-3): 1. Earthquake 2. Typhoon 3. Flood"
  input disaster
  display "Choose a setting (home / school / street): "
  input setting

  if disaster == 1 and (setting == "home" or setting == "school")
    earthquake()
  if disaster == 1 and setting == "street"
    earthquakestreet()
  if disaster == 2 and setting == "home"
    typhoonhome()

  end function

function earthquake()
  Display "You are at ", setting, " and the ground starts shaking aggresively! What do you do? (enter 1-2)"
  Display "1. Hide under a sturdy table and cover your head."
  Display "2. Run outside to find adults and seek guidance."
  input choice1
  
  if choice1 == 1 then
    display "The shaking intensifies! what do you do? (enter 1-2)"
    display "1. Curl up and protect your head and neck."
    display "2. Rush outside to seek for help from adults."
    input choice2

    if choice2 == 1 then
      display "The ground stopped shaking. You were protected from broken glass and falling debris. You survived with no injuries!"
    else then
      display "You tripped while running outside and pieces of debris fell on you! The shaking stops but you were heavily injured."

  else then
    display "You fell and twisted your ankle while running to the outside. What do you do? (enter 1-2)"
    display "1. Do your best to keep running to get out of the house and seek medical attention."
    display "2. Duck and stay away from windows. You crawl under a sturdy structure and protect your head."
    input choice3

    if choice3 == 1 then
      display "You finally made it outside."
      display "Look out! A car lost its control and it's coming for you!"
      display "... You died."

    else then
      display "The ground stopped shaking. Your ankle aches but you were safe. Eventually, you were given medical attention. Good job!"

  end function

  funtion earthquakestreet()
    Display "You are walking outside when the ground starts shaking aggressively! What will you do?(enter 1-3)"
    Display "1. Walk away from the buildings and cars. You kneel down and cover your head with a bag."
    Display "2. Run inside the nearest store to hide under a sturdy structure and protect yourself."
    display "3. Lean on a wall while covering your head to find support for balance."
    input choice4

    if choice4 == 1 then
      display "People shouted around you as the cars honked. You were hit with a few pieces of debris but you came out of the earthquake alive."

    if choice4 == 2 then
      display "Debris fell on your head when you reached the entrance! Your head starts throbbing. What do you do? (enter 1-2)"
      display "1. Crawl to a sturdy structure and hide."
      display "2. Go back outside to the streets."
      input choice5

      if choice5 == 1 then
        display "The glass shatters and so do the lights. However, you were safe. The earthquake passed and despite your minor head injury, you survived!"
      else then
        display "You were hit by shattering glass and more debris. Your vision slowly starts fading..."
        display "You opened your eyes to the blinding lights of a hospital. The earthquake passed. You were heavily injured but you survived."

      if choice4 == 3
        display "A large pile of debris hit you! You lose consciousness and never gained it back again."

    end function

    function typhoonhome()
      display "It has been raining heavily for a while. Your anxiety was slowly rising. What do you do?"
      display "1. Watch the news with your family."
      display "2. Distract yourself by playing games and staying positive."
      input choice6

      if choice6 == 1
        display "The news reporter said a strong typhoon was heading to your province! What do you do?"
        display "1. Prepare an emergency bag and try to search up an evacuation plan."
        display "2. Leave it be. It'll pass. What's most important is staying calm."
        input choice7

        if choice7 == 1
          display "You packed all the essentails. What now?"
          display "1. Run away to find authorities who can protect and guide you."
          display "2. Follow your parents upstairs."
          input choice8

          if choice8 == 1
            display "The wind was too strong, but you were determined. The trees shook around, it was normal under these conditions."
            display "You saw a tree falling straight towards you, and boom!"
            display "You died."

          if choices8 == 2
            display ""

        if choice7 == 2
          display "You were completely unprepared. What will you do now?"

    

  
  
      


  
