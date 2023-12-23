local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()

local Window = Library.CreateLib("Viet nam piece", "DarkTheme")

local Tab = Window:NewTab("Main")
local Section = Tab:NewSection("Farm")
------------------------
------------------------
Section:NewButton("Farm", "", function()
_G.farm = true;
while _G.farm do wait()
pcall(function ()
for i,v in pairs(game:GetService("Workspace")["NPC DAMAGE"]:GetDescendants()) do
	if v.Name == "Sukuna" then
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,0,8)
			end
		end
	end)
end
end)
Section:NewButton("Stop Farm", "", function()
_G.farm = false;
while _G.farm do wait()
pcall(function ()
for i,v in pairs(game:GetService("Workspace")["NPC DAMAGE"]:GetDescendants()) do
	if v.Name == "Sukuna" then
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,0,8)
			end
		end
	end)
end
end)
-------------------
local Section = Tab:NewSection("click")
Section:NewButton("click", "", function()
_G.click = true;
while _G.click do wait(0)
local args = {
    [1] = 8,
    [2] = 1
}
game:GetService("Players").LocalPlayer.Character.YorusV3.Hitbox:FireServer(unpack(args))
end
end)
--------------------------------
local Section = Tab:NewSection("Quest")
Section:NewButton("Auto Quest", "", function()
_G.loop = true;
while _G.loop do wait()
workspace:FindFirstChild("Cursed Island [  50000+ ]"):FindFirstChild("Sukuna Quest [ Lv 50.000+ ]").Quest.QuestTake.QuestTake.Accept2.RemoteEvent:FireServer()
end
end)
Section:NewButton("Stop Quest", "", function()
_G.loop = false;
while _G.loop do wait()
workspace:FindFirstChild("Cursed Island [  50000+ ]"):FindFirstChild("Sukuna Quest [ Lv 50.000+ ]").Quest.QuestTake.QuestTake.Accept2.RemoteEvent:FireServer()
end
end)


local Section = Tab:NewSection("KAIDO")

Section:NewButton("Farm", "", function()
_G.farmKaidou = true;
while _G.farmKaidou do wait()
pcall(function ()
for i,v in pairs(game:GetService("Workspace")["NPC DAMAGE"]:GetDescendants()) do
	if v.Name == "Kaidou" then
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,0,3)
			end
		end
	end)
end
end)
Section:NewButton("Stop Farm", "", function()
_G.farmKaidou = false;
while _G.farmKaidou do wait()
pcall(function ()
for i,v in pairs(game:GetService("Workspace")["NPC DAMAGE"]:GetDescendants()) do
	if v.Name == "Kaidou" then
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,0,3)
			end
		end
	end)
end
end)

Section:NewButton("Auto Quest KAIDO", "", function()
_G.KAIDO = true;
while _G.KAIDO do wait()
workspace:FindFirstChild("Kaido Island [ Lv 1000+ ]"):FindFirstChild("KAIDOUU QUESTTT").ClickPart.QuestTake.QuestTake.Accept1.RemoteEvent:FireServer()
end
end)
Section:NewButton("Stop Quest KAIDO", "", function()
_G.KAIDO = false;
while _G.KAIDO do wait()
workspace:FindFirstChild("Kaido Island [ Lv 1000+ ]"):FindFirstChild("KAIDOUU QUESTTT").ClickPart.QuestTake.QuestTake.Accept1.RemoteEvent:FireServer()
end
end)
