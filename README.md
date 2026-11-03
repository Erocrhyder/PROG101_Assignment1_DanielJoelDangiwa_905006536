# PROG101_Assignment1_DanielJoelDangiwa_905006536
This is assignment 1 for Programming Logic and Design about a Community Flood Alert and Response system in Sierra Leone

# Pseudocode of the system
Function Main
    Declare String ObservationDateTime, UpdateDateTime, Location, UserContactInformation
    Declare String ContinousHeavyRain, RapidRise, WaterDisruption, ImmediateDanger, DrainOverflow, TidalOverflow, WaterAccumulation, BuildingInfiltration
    Declare Integer UserChoice

    Output "Welcome to the Community Flood Alert and Response Information System (CFARIS)"
    Output "Kindly choose from the options below"
    Output "1. Submit a flood report" & ToChar(13) & "2. Check The Latest Update" & ToChar(13) & "3. Exit"
    Input UserChoice
    If UserChoice==1
        Output "You've chosen to submit a flood report."
        Output "Please enter the name of the location that has been affected."
        Input Location
        Output "When was this observed?"
        Input ObservationDateTime
        Output "Thank you for your valued input, kindly answer the following questions with 'Yes' or 'No' based on what you observed"
        Output "Has heavy rain been falling continously in or near the affected area?"
        Input ContinousHeavyRain
        Output "Have nearby rivers, streams, or drainage channels risen noticeably above their usual levels?"
        Input RapidRise
        Output "Are drains or waterways blocked, overflowing, or unable to carry away rainwater?"
        Input DrainOverflow
        Output "Has floodwater entered an occupied building in the affected area?"
        Input BuildingInfiltration
        Output "Is water beginning to accumulate in low-lying areas or on roads?"
        Input WaterAccumulation
        Output "Has water been observed disrupting routes or community services (Schools, Clinics, businesses, etc)?"
        Input WaterDisruption
        Output "Is anyone trapped, injured, or in immediate danger because of the flooding"
        Input ImmediateDanger
        If ImmediateDanger=="Yes" OR BuildingInfiltration=="Yes"
            Output "Risk Assessment: Urgent"
            Output "Area: " & Location & ToChar(13) & "Risk Assessment: Urgent" & ToChar(13) & "Observation Date & Time: " & ObservationDateTime & ToChar(13) & "Safety Guidance: Move away from affected areas and to a safer place if you can, do not walk or drive through floodwater. If anyone is trapped, injured, or in immediate danger, contact local emergency services or authorities (Call NDMA toll-free: 1199)."
        Else
            If RapidRise=="Yes" OR DrainOverflow=="Yes" OR WaterDisruption== "Yes"
                Output "Risk Assessment: Warning"
                Output "Area: " & Location & ToChar(13) & "Risk Assessment: Warning" & ToChar(13) & "Observation Date & Time: " & ObservationDateTime & ToChar(13) & "Safety Guidance: Avoid drains and floodwater, follow local emergency instructions and stay alert for changing conditions"
            Else
                If ContinousHeavyRain=="Yes" OR WaterAccumulation=="Yes"
                    Output "Risk Assessment: Advisory"
                    Output "Area: " & Location & ToChar(13) & "Risk Assessment: Advisory" & ToChar(13) & "Observation Date & Time: " & ObservationDateTime & ToChar(13) & "Safety Guidance: Prepare to move to a safer place if conditions worsen and follow local emergency instructions if given, avoid reported flood-prone areas and affected routes"
                Else
                    If ImmediateDanger=="No" AND BuildingInfiltration=="No" AND DrainOverflow=="No" AND WaterDisruption=="No" AND ContinousHeavyRain=="No" AND WaterAccumulation=="No" AND RapidRise=="No"
                        Output "Risk Assessment: Safe"
                        Output "Area: " & Location & ToChar(13) & "Risk Assessment: Safe" & ToChar(13) & "Observation Date & Time: " & ObservationDateTime & ToChar(13) & "Safety Guidance: No immediate signs of flooding were reported but this does not guarantee safety, continue to monitor the environment and follow any officisl instructions"
                    Else
                        Output "Risk Assessment: Unclear"
                        Output "Area: " & Location & ToChar(13) & "Risk Assessment: Unclear" & ToChar(13) & "Observation Date & Time: " & ObservationDateTime & ToChar(13) & "Safety Guidance: Information was unclear and there is not enough information to assess the situation."
                    End
                End
            End
        End
    Else
        If UserChoice==2
            Output "Please enter the area you would like to check"
            Input Location
            Output "Area: " & Location & ToChar(13) & "Risk Assessment: " & "Safe" & ToChar(13) & "Observation Date & Time: " & "25 October 2026, 10:00 AM" & ToChar(13) & "Safety Guidance (At time of update): No immediate signs of flooding were reported but this does not guarantee safety. Continue to monitor the environment and follow any official instructions"
        Else
            If UserChoice==3
                Output "You have chosen to exit."
            Else
                Output "Your input was invalid, please try again next time."
            End
        End
    End
    Output "Thank you for using the Community Flood Alert and Response Information System. Goodbye."
    End
  # Flowchart of the system
  <img width="1918" height="976" alt="Flowchart screenshot 1" src="https://github.com/user-attachments/assets/ea2947d5-4125-473a-acbc-cd7889425a27" />
<img width="1917" height="982" alt="Flowchart screenshot 2" src="https://github.com/user-attachments/assets/8e332819-78fe-4ce1-bfc6-37ee5711b306" />
<img width="1920" height="977" alt="Flowchart screenshot 3" src="https://github.com/user-attachments/assets/8d1f2d2d-b74e-417b-bca4-80f8538ebb27" />
<img width="1917" height="975" alt="Flowchart screenshot 4" src="https://github.com/user-attachments/assets/64f35367-d08f-4dfc-b075-803116fad64d" />
<img width="1907" height="952" alt="Flowchart Screenshot 5" src="https://github.com/user-attachments/assets/91d9012f-e9a8-4fb9-a803-be348f54f676" />
<img width="1157" height="850" alt="Flowchart Screenshot 6" src="https://github.com/user-attachments/assets/55597f1f-da65-495f-a5ba-37d28473f85f" />
<img width="1060" height="852" alt="Flowchart Screenshot 7" src="https://github.com/user-attachments/assets/80c92e0d-91d4-4d08-b3b8-afb9a51c9698" />
<img width="1917" height="260" alt="Flowchart Screenshot 8" src="https://github.com/user-attachments/assets/ef9ebcde-ec88-4531-9873-22b3d9555f72" />
