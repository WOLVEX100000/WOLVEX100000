local library = loadstring(game:HttpGet(('https://raw.githubusercontent.com/bloodball/-back-ups-for-libs/main/wall%20v3')))()

local w = library:CreateWindow("WolveX's GUI")

local b = w:CreateFolder("Scripts") -- Creates the folder(U will put here your buttons,etc)

b:Label("Sword Simulator",{

    TextSize = 25;

    TextColor = Color3.fromRGB(255,255,255); -- Self Explaining

    BgColor = Color3.fromRGB(69,69,69); -- Self Explaining

    

})

b:Button("Auto Heal",function()

    while wait () do

workspace.__EVENTS.Loader:FireServer()

workspace.__EVENTS.Re:FireServer()

workspace.__EVENTS.He:FireServer()

workspace.__EVENTS.Heal:FireServer()

end

end)

b:Button("GodMode",function()

   while wait() do

game.Players.LocalPlayer.Character.pvp:Destroy()

end

end

end)

b:Button("Dark SS Gui",function()

    loadstring(game:HttpGet(("https://raw.githubusercontent.com/SukiScripts/DarkDestroyer/main/DarkGui"), true))()

--creator: Suki And Wolve

--Btw This is V2 Join Our DIscord Server! https://discord.gg/w3mYRWuWRq

end)

b:Button("Faizan Destroyer",function()

    local A_1 = game.Players.LocalPlayer.name.." Loaded Faizan's Destroyer"-----message here

local A_2 = "All"

local Event = game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest

Event:FireServer(A_1, A_2)

loadstring(game:HttpGet(("https://raw.githubusercontent.com/SukiScripts/FaizansGui/main/Faizan"), true))()

--creator: Alex And Faizan

--Btw This is V1 Join Our DIscord Server! https://discord.gg/w3mYRWuWRq

end)

b:Button("Infinite Yield",function()

    loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()

end)

b:Button("Liquid Gui",function()

    loadstring(game:HttpGet(("https://raw.githubusercontent.com/SukiScripts/Liquid/main/LiquidGuiFULL"), true))()

--creator: WolveX AKA Scriptliner

end)

b:Button("Sword Spin",function()

while true do

        local player = game.Players.LocalPlayer

        local character = player.Character

        local backpack = player.Backpack

        local swords = {}

        function look(dir)

            for i, v in pairs(dir:GetChildren()) do

                if(v:IsA("Tool"))then

                    table.insert(swords,v)

                end

            end

        end

        look(backpack)

        look(character)

        for i, v in pairs(swords)do

            local sword             = v

            sword.Parent            = backpack

            sword.Handle.Massless   = true

            sword.Handle.CanCollide = true

            sword.Grip              = (sword.Grip*CFrame.Angles(1.50,0,0))*CFrame.new(0,0,0.5*(i-1))

            sword.Parent            = character

            sword.Handle.Touched:Connect(function(t)

                if(t.Parent)and(t.Parent:FindFirstChild("Humanoid"))and(t.Parent.Name~=player.Name)then

                    sword.Handle.dmg.RemoteEvent:FireServer(t.Parent.Humanoid, math.huge)

                end

            end)

        end

        wait(0.1)

    end

    

end)

local A_1 = game.Players.LocalPlayer.name.." Loaded WolveX's SS Gui "-----message here

        local A_2 = "All"

        local Event = game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest

        Event:FireServer(A_1, A_2)

local b = w:CreateFolder("Scripts") -- Creates the folder(U will put here your buttons,etc)

b:Label("Sword Simulator",{

    TextSize = 25;

    TextColor = Color3.fromRGB(255,255,255); -- Self Explaining

    BgColor = Color3.fromRGB(69,69,69); -- Self Explaining

    

})




 
