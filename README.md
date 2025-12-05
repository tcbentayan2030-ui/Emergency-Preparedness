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
- Firstly, the user will choose a setting, and disaster, which are prompted by the pogram. The program will then return a scenario with the chosen disaster and setting and will ask the user to make choices, depeding on the scenario. It will result in different endings depending on the choices the user made throughout the game.

Logic Plan:
Psuedocode:

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

  if disaster == 2 and setting == "school" then
    typhoonschool()
  end if

  if disaster == 3 and setting == "home" then
    floodhome()
  end if

  if disaster == 3 and setting == "street" then
    floodstreet()
  end if

  if disaster == 3 and setting == "school" then
    floodschool()
  end if

end function


function earthquake(setting)
  display "You are at ", setting, " and the ground starts shaking aggressively! (enter 1-2)"
  display "1. Hide under a sturdy table."
  display "2. Run outside."
  input choice1

  if choice1 == 1 then
    display "The shaking intensifies! (enter 1-2)"
    display "1. Curl up and protect your head."
    display "2. Rush outside."
    input choice2

    if choice2 == 1 then
      display "The ground stopped shaking. You survived with no injuries!"
    else
      display "You tripped while running outside. Debris fell on you. You were heavily injured."
    end if

  else
    display "You fell and twisted your ankle while running. (enter 1-2)"
    display "1. Keep running."
    display "2. Crawl to safety indoors."
    input choice3

    if choice3 == 1 then
      display "A car lost control and hit you. You died."
    else
      display "The ground stopped shaking. You stayed safe and were later treated."
    end if
  end if

end function


function earthquakestreet()
  display "You are walking outside when the ground starts shaking! (enter 1-3)"
  display "1. Move away from buildings, kneel, cover your head."
  display "2. Run into a store."
  display "3. Lean on a wall."
  input choice4

  if choice4 == 1 then
    display "You were hit by small debris but survived."
  end if

  if choice4 == 2 then
    display "Debris hits your head at the store entrance! (enter 1-2)"
    display "1. Crawl to a sturdy structure."
    display "2. Go back outside."
    input choice5

    if choice5 == 1 then
      display "Glass shattered but you survived with a minor head injury."
    else
      display "More debris hit you outside. You woke up in a hospital but survived."
    end if
  end if

  if choice4 == 3 then
    display "A pile of debris fell on you. You died."
  end if
end function



function typhoonhome()
  display "Dark clouds loom. What do you do? (enter 1-2)"
  display "1. Watch the news with your family."
  display "2. Distract yourself by playing games."
  input choice6

  if choice6 == 1 then
    display "A typhoon is coming. Prepare your emergency kit. (enter 1-2)"
    display "1. Run outside to find authorities."
    display "2. Unplug appliances and go upstairs."
    input choice7

    if choice7 == 1 then
      display "The wind is too strong. A tree falls toward you... You died."
    else
      display "Water begins to rise. What now? (enter 1-3)"
      display "1. Watch news via radio / phone."
      display "2. Watch news via TV."
      display "3. Open the window to look outside."
      input choice8

      if choice8 == 1 then
        display "According to the news reposter, the typhoon will last for two days."
        display "Thankfully, you packed food and water. You survived!"
      end if

      if choice8 == 2 then
        display "Power surge! You were electrocuted. You died."
      end if

      if choice8 == 3 then
        display "The window shattered and injured you. Thankfully, you packed for first aid."
        display "The typhoon lasted for 2 days but with your food, water, and supplies, you survived perfectly!"
      end if
    end if

  else
    display "You didn’t notice water entering the house! (enter 1-2)"
    display "1. Run outside to find authorities."
    display "2. Unplug outlets and go upstairs."
    input choice9

    if choice9 == 1 then
      display "The wind is too strong. A tree falls toward you... You died."
    else
      display "You are now upstairs. What next? (enter 1-3)"
      display "1. Watch news via radio / phone."
      display "2. Watch news via TV."
      display "3. Open the window to check outside."
      input choice10

      if choice10 == 1 then
        display "You survived, dehydrated and starving."
      end if

      if choice10 == 2 then
        display "Power surge! You were electrocuted. You died."
      end if

      if choice10 == 3 then
        display "Window shattered. Several fragments cut through you, but you didn't pack first aid."
        display "You survived with a few injuries."
      end if
    end if
  end if

end function



function typhoonstreet()
  display "Heavy rain starts. What do you do? (enter 1-2)"
  display "1. Find authorities."
  display "2. Go home."
  input choice11

  if choice11 == 2 then
    typhoonhome()
  end if

  if choice11 == 1 then
    display "The wind is too strong. A tree falls toward you... You died."
  end if

end function



function typhoonschool() 
display "Dark clouds gather outside. Your teacher announces that a typhoon is approaching. What do you do? (enter 1-2)" 
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
  display "It's been raining for hours. Water is rising. (enter 1-2)"
  display "1. Check the news."
  display "2. Ignore it."
  input choice17

  if choice17 == 1 then
    display "Severe flood warning! Prepare the emergency kit. (enter 1-2)"
    display "1. Prepare the kit properly."
    display "2. Pack a few items and rush upstairs."
    input choice18

    if choice18 == 1 then
      display "Floodwater enters the house! (enter 1-2)"
      display "1. Go upstairs."
      display "2. Go outside for rescuers."
      input choice19

      if choice19 == 1 then
        display "You are upstairs. (enter 1-3)"
        display "1. Listen to radio updates."
        display "2. Look out the window."
        display "3. Try to wade to a neighbor."
        input choice20

        if choice20 == 1 then
          display "Rescuers eventually arrived. You survived!"
        end if

        if choice20 == 2 then
          display "Debris breaks the window. You are cut but survive."
        end if

        if choice20 == 3 then
          display "The current pulls you away. You drowned."
        end if

      else   // choice19 == 2
        display "A surge of water hits you when you open the door. You are swept away. You died."
      end if

    else
      display "You rushed upstairs but forgot essentials. (enter 1-3)"
      display "1. Use phone flashlight and stay put."
      display "2. Go downstairs for items."
      display "3. Signal from the window."
      input choice21

      if choice21 == 1 then
        display "Rescuers arrived. You survived but were cold and hungry."
      end if

      if choice21 == 2 then
        display "Water too high; you slipped and drowned."
      end if

      if choice21 == 3 then
        display "Neighbors signaled rescuers. You survived."
      end if
    end if

  else
    display "You ignored the rain. Water rushes inside! (enter 1-2)"
    display "1. Run outside."
    display "2. Go upstairs."
    input choice22

    if choice22 == 1 then
      display "Current too strong; you were swept away. You died."
    else
      display "You are upstairs without supplies. (enter 1-2)"
      display "1. Wait for rescue."
      display "2. Signal for help."
      input choice23

      if choice23 == 1 then
        display "You survived but exhausted and dehydrated."
      else
        display "A rescue boat saw your signal. You survived!"
      end if
    end if

  end if

end function


function floodstreet()
  display "Rain intensifies. Water is rising. (enter 1-2)"
  display "1. Look for higher ground."
  display "2. Try to walk home."
  input choice24

  if choice24 == 1 then
    display "You climbed to higher ground. (enter 1-2)"
    display "1. Wait for rescue."
    display "2. Try running home."
    input choice25

    if choice25 == 1 then
      display "Rescue vehicle found you. You survived!"
    else
      display "Flood surge hits suddenly. You died."
    end if

  else
    display "Water reaches your knees. (enter 1-2)"
    display "1. Keep pushing toward home."
    display "2. Retreat to higher ground."
    input choice26

    if choice26 == 1 then
      display "Strong currents swept you away. You died."
    else
      display "You waited on high ground and were rescued. You survived!"
    end if
  end if

end function


function floodschool()
  display "School grounds are flooding. (enter 1-2)"
  display "1. Go home as instructed."
  display "2. Stay inside the classroom."
  input choice27

  if choice27 == 1 then
    display "You pack your things and leave the school."
    floodhome()
  else
    display "Floodwater enters the school! (enter 1-2)"
    display "1. Move to the second floor."
    display "2. Hide under a desk."
    input choice28

    if choice28 == 1 then
      display "You remained safe upstairs. Rescuers arrived later. You survived!"
    else
      display "Floodwater rose too fast. You drowned."
    end if
  end if

end function


main()




    
  


          
        
            

    

  
  
      


  
