# Emergency-Preparedness
This game will test you on your decision-making in the face of disasters. Be wise in your choices to survive the disaster.

Project Title
- Emergency Preparedness: Test Your Choices during Disasters

Problem Statement
- You can't stop disasters from happening all around the world at any point of the day, but you can control how you respond to it. Those who are unaware of what to do during those times are more likely to face grave injuries and death.

Project Objectives
- Our program will help users understand what to do during different disasters of their choosing through an interactive game where they make choices based on the given scenario and disaster. This can help in spreading awareness and facts about disasters so that more peaople can have a better understanding on how every action can affect them during those times.

Planned Features
-  Our program will use built-in commands, functions, etc. to make our game interactive and fun.

Planned Inputs and Outputs
- Firstly, the user will a setting, and disaster, which are prompted by the pogram. The program will then return a scenario with the chosen disaster and setting and will ask the user to make choices, depeding on the scenario. It will result in different endings depending on the choices the user made throughout the game.

Logic Plan:
Psuedocode:

start program

function main()
  display "Welcome to our game where we will test your ability to make the right decisions during disasters."
  display "Pick a disaster (enter 1-3): 1. Earthquake 2. Typhoon 3. Flood"
  input disaster

  display "Choose a setting (home / school / street): "
  input setting

  if disaster == 1 and (setting == "home" or setting == "school") then
    earthquake(setting)
  end if

  if disaster == 1 and setting == "street" then
    earthquakestreet()
  end if

  if disaster == 2 and setting == "home" then
    typhoonhome()
  end if

  if disaster == 2 and setting == "street" then
    typhoonstreet()
  end if

end function


function earthquake(setting)
  display "You are at ", setting, " and the ground starts shaking aggressively! What do you do? (enter 1-2)"
  display "1. Hide under a sturdy table and cover your head."
  display "2. Run outside to find adults and seek guidance."
  input choice1

  if choice1 == 1 then
    display "The shaking intensifies! What do you do? (enter 1-2)"
    display "1. Curl up and protect your head and neck."
    display "2. Rush outside to seek help from adults."
    input choice2

    if choice2 == 1 then
      display "The ground stopped shaking. You were protected from broken glass and falling debris. You survived with no injuries!"
    else
      display "You tripped while running outside and debris fell on you! You were heavily injured."
    end if

  else
    display "You fell and twisted your ankle while running outside. What do you do? (enter 1-2)"
    display "1. Keep running to get out of the house and seek medical attention."
    display "2. Duck and stay away from windows. Crawl under a sturdy structure and protect your head."
    input choice3

    if choice3 == 1 then
      display "You finally made it outside."
      display "Look out! A car lost control and it's coming for you!"
      display "... You died."
    else
      display "The ground stopped shaking. Your ankle aches but you were safe. You eventually received medical attention. Good job!"
    end if
  end if

end function


function earthquakestreet()
  display "You are walking outside when the ground starts shaking aggressively! What will you do? (enter 1-3)"
  display "1. Walk away from buildings and cars, kneel down, and cover your head."
  display "2. Run inside the nearest store to hide."
  display "3. Lean on a wall while covering your head."
  input choice4

  if choice4 == 1 then
    display "People shouted as cars honked. You were hit by small debris but survived."
  end if

  if choice4 == 2 then
    display "Debris fell on your head at the entrance! Your head throbs. What do you do? (enter 1-2)"
    display "1. Crawl to a sturdy structure and hide."
    display "2. Go back outside to the streets."
    input choice5

    if choice5 == 1 then
      display "The glass shattered and so did the lights. However, you were safe and survived with a minor head injury."
    else
      display "You were hit by more shattering glass and debris. You woke up in a hospital—injured but alive."
    end if
  end if

  if choice4 == 3 then
    display "A pile of debris hit you! You lose consciousness and never wake up again."
  end if

end function


function typhoonhome()
  display "Thick, dark clouds overshadow the sky. Your anxiety rises. What do you do? (enter 1-2)"
  display "1. Watch the news with your family."
  display "2. Distract yourself by playing games."
  input choice6

  if choice6 == 1 then
    display "The news reporter says a typhoon is coming!"
    display "They tell you to pack an emergency kit."
    display "You packed all essentials. What now? (enter 1-2)"
    display "1. Run outside to find authorities."
    display "2. Unplug all outlets and go upstairs."
    input choice7

    if choice7 == 1 then
      display "The wind is too strong. A tree falls toward you..."
      display "...You died."
    else
      display "Water starts rising but you are safe upstairs."
      display "What now? (enter 1-3)"
      display "1. Watch the news via phone or radio."
      display "2. Watch news via television."
      display "3. Open the window to see outside."
      input choice8

      if choice8 == 1 then
        display "The typhoon will last two more days. Luckily, you have food. You survived!"
      end if

      if choice8 == 2 then
        display "A power surge occurred when you plugged in the TV. You were electrocuted!"
        display "You died."
      end if

      if choice8 == 3 then
        display "The window shattered and injured you! But you had first-aid. You survived with cuts."
      end if

    end if

  else
    display "You didn’t notice water entering the house! What now? (enter 1-2)"
    display "1. Run outside to find authorities."
    display "2. Unplug outlets and go upstairs."
    input choice9

    if choice9 == 1 then
      display "The wind is too strong. A tree falls toward you..."
      display "...You died."
    else
      display "Water rises but you are safe upstairs."
      display "What now? (enter 1-3)"
      display "1. Watch news via phone or radio."
      display "2. Watch news via television."
      display "3. Open the window to check outside."
      input choice10

      if choice10 == 1 then
        display "The typhoon will last two more days. You had no food or water. You survived but severely dehydrated and starving."
      end if

      if choice10 == 2 then
        display "A power surge electrocuted you!"
        display "You died."
      end if

      if choice10 == 3 then
        display "The window shattered and injured you."
        display "You survived but your wounds almost got infected and you were severely dehydrated and starving."
      end if
    end if
  end if

end function

function typhoonstreet()
  display "You were walking in the streets, just near your house, when the heavy rain started. What will you do?(enter 1-2)"
  display "1. Find authorities."
  display "2. Go home."
  input choice11

  if choice11 == 2
    function typhoonhome()
  if choice11 == 1
    display "The wind is too strong. A tree falls toward you..."
    display "...You died."
  end if

function typhoonschool()
  display "Dark clouds gather outside as the winds start to howl. Your teacher announces that a typhoon is approaching. What do you do? (enter 1-2)"
  display "1. Listen carefully to your teacher’s instructions."
  display "2. Panic and rush to the hallway to look for your friends."
  input choice12

  if choice12 == 1 then
    display "Your teacher instructs everyone to stay calm and move to a safer classroom away from windows."
    display "What will you do? (enter 1-2)"
    display "1. Follow the teacher and stay with your class."
    display "2. Sneak back to the original classroom to get your phone."
    input choice13

    if choice13 == 1 then
      display "The wind outside grows stronger. The windows rattle loudly."
      display "Your teacher tells everyone to duck, cover, and hold. What do you do? (enter 1-2)"
      display "1. Duck under a sturdy desk and cover your head."
      display "2. Move closer to the windows to see what's happening outside."
      input choice14

      if choice14 == 1 then
        display "The glass shattered but you were protected by the desk."
        display "Rescue teams later arrived and evacuated your class safely. You survived with no injuries!"
      else
        display "The wind blew debris through the window!"
        display "You were struck by shards of glass. Your classmates helped you, but you were heavily injured."
      end if

    else
      display "You sneaked back to get your phone."
      display "Suddenly, the wind shattered the classroom window and debris flew inside!"
      display "You were knocked unconscious."
      display "Hours later, rescuers found you and rushed you to a hospital. You survived, but badly injured."
    end if


  else 
    display "You ran into the hallway. The lights flickered and the rain fell loudly outside."
    display "A teacher spotted you and yelled for you to return to class. What do you do? (enter 1-2)"
    display "1. Ignore them and keep running to look for your friends."
    display "2. Go back to the classroom like they said."
    input choice15

    if choice15 == 1 then
      display "A strong gust of wind caused part of the ceiling to fall in the hallway!"
      display "You were caught under falling debris... You died."
    else
      display "You ran back to the classroom."
      display "Your teacher immediately guided you to safety."
      display "What do you do now? (enter 1-2)"
      display "1. Follow their instructions and duck under a desk."
      display "2. Sit frozen and refuse to move."
      input choice16

      if choice16 == 1 then
        display "The storm intensified, but you stayed safe under the desk."
        display "The typhoon passed, and emergency services evacuated your school. You survived!"
      else
        display "You sat frozen near the center of the room."
        display "A large piece of debris fell from the ceiling and hit you!"
        display "You were seriously injured, but later rescued."
      end if

    end if
  end if

end function

function floodhome()
  display "It's been raining nonstop for hours. The water outside is rising quickly. What do you do? (enter 1-2)"
  display "1. Check the news and weather updates."
  display "2. Ignore it and continue with your day."
  input choice17

  if choice17 == 1 then
    display "The news reports a severe flood warning in your area!"
    display "Your parents tell you to prepare the emergency kit. What do you do? (enter 1-2)"
    display "1. Help prepare the emergency kit thoroughly."
    display "2. Only pack a few items and rush upstairs immediately."
    input choice18

    if choice18 == 1 then
      display "The floodwater begins entering the house! What now? (enter 1-2)"
      display "1. Go upstairs and stay calm."
      display "2. Go outside to look for rescuers."
      input choice19

      if choice19 == 1 then
        display "You're upstairs and safe for now. The water rises but doesn't reach the second floor."
        display "What do you do next? (enter 1-3)"
        display "1. Listen to the radio for updates."
        display "2. Look out the window to check the situation."
        display "3. Attempt to wade through the water to reach your neighbor."
        input choice20

        if choice20 == 1 then
          display "The news says rescuers are on the way. You stay put and conserved your supplies."
          display "After several hours, rescuers help you out. You survived with no injuries!"
        end if

        if choice20 == 2 then
          display "A strong current bangs debris against the window!"
          display "Glass shatters and you get cuts, but your first-aid kit helps. You survive with minor injuries."
        end if

        if choice20 == 3 then
          display "The floodwater outside is stronger than you expected!"
          display "The current pulls you and drags you away..."
          display "...You drowned."
        end if

      if choice19 == 2
        display "You open the door and a strong surge of water hits you!"
        display "You get swept away by the current..."
        display "...You died."
      end if


    if choice18 == 2
      display "You rushed upstairs but forgot many essentials."
      display "The water keeps rising and the power goes out."
      display "What do you do? (enter 1-3)"
      display "1. Use your phone’s flashlight and stay put."
      display "2. Try to grab items downstairs."
      display "3. Try shouting from the window for help."
      input choice21

      if choice21 == 1 then
        display "You conserved your energy and waited."
        display "Rescuers eventually arrived. You survived, but you're cold and hungry."
      end if

      if choice21 == 2 then
        display "You attempt to go downstairs, but the water is already too high."
        display "You slip and get pulled underwater..."
        display "...You died."
      end if

      if choice21 == 3 then
        display "A neighbor hears you and signals rescue workers."
        display "You were eventually rescued, shaken but alive."
      end if

    end if


  else  // choice17 == 2
    display "You ignored the rain... but water suddenly rushes into the house!"
    display "You're caught off guard. What do you do? (enter 1-2)"
    display "1. Run outside to escape the flood."
    display "2. Go upstairs immediately."
    input choice22

    if choiceF6 == 1 then
      display "You waded outside, but the current was much stronger than you expected."
      display "The water knocked you off your feet..."
      display "...You died."
    else
      display "You rushed upstairs just in time."
      display "However, you didn’t bring supplies. What now? (enter 1-2)"
      display "1. Stay calm and wait for rescue."
      display "2. Try signaling for help through the window."
      input choice23

      if choice23 == 1 then
        display "You waited for hours with no food or water."
        display "Eventually, rescuers reached your home. You survived—but exhausted and dehydrated."
      else
        display "You shouted for help. A nearby rescue boat noticed your flashlight signal."
        display "They rescued you safely. Good job!"
      end if

    end if

  end if

end function

function floodstreet()
  display "You're walking home when the rain intensifies. Water starts rising quickly along the street. What do you do? (enter 1-2)"
  display "1. Look for higher ground nearby."
  display "2. Continue walking home before it gets worse."
  input choice24

  if choice24 == 1 then
    display "You climbed to higher ground. The water keeps rising."
    display "A rescue vehicle spots you. What do you do? (enter 1-2)"
    display "1. Wait for rescue."
    display "2. Try running home while the road looks clear."
    input choice25

    if choice25 == 1 then
      display "You stayed safe and were rescued. You survived!"
    else
      display "The 'clear' road suddenly floods with a strong surge of water..."
      display "...You died."
    end if

  if choice24 == 2 (go home)
    display "The water rises to your knees. What now? (enter 1-2)"
    display "1. Keep pushing toward home."
    display "2. Retreat to higher ground."
    input choice26

    if choice26 == 1 then
      display "A strong current swept you off your feet."
      display "...You died."
    else
      display "You reached higher ground and waited."
      display "Rescuers eventually brought you home safely. You survived!"
    end if

  end if

end function

function floodschool()
  display "Rain pours heavily and the water in the school grounds begins rising quickly."
  display "Your teacher receives instructions from the principal."
  display "Students who can safely get home are advised to go home immediately."
  display "What do you do? (enter 1-2)"
  display "1. Go home as instructed."
  display "2. Stay inside the classroom and wait for the flood to pass."
  input f27

  if f27 == 1 then
    display "You pack your things quickly and leave the school."
    floodhome()

  if choice27 == 2
    display "You decide to stay inside the school even though it's not recommended."
    display "The water outside rises fast and starts entering the classrooms!"
    display "What do you do? (enter 1-2)"
    display "1. Move to the second floor with remaining students."
    display "2. Hide under a desk and hope for the best."
    input choice28

    if choice28 == 1 then
      display "You move to the second floor and stay dry."
      display "Hours pass. The water remains high, but rescuers eventually arrive."
      display "You survived, but were stranded at school for a long time."
    else
      display "The water floods the first floor rapidly!"
      display "Debris floats inside and knocks you over..."
      display "...You drowned."
    end if

  end if

end function

main()



    
  


          
        
            

    

  
  
      


  
