-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local Main = Instance.new("Frame")
local Side = Instance.new("Frame")
local Navigation = Instance.new("Frame")
local Dash = Instance.new("Frame")
local scriptFrame = Instance.new("Frame")
local Frame = Instance.new("Frame")
local Logo = Instance.new("TextLabel")
local Version = Instance.new("TextLabel")
local Logo2 = Instance.new("TextLabel")
local DT = Instance.new("TextLabel")
local SHT = Instance.new("TextLabel")
local Eth = Instance.new("TextLabel")
local TextLabell = Instance.new("TextLabel")
local Namee = Instance.new("TextLabel")
local Close = Instance.new("TextButton")
local EspName = Instance.new("TextButton")
local Fullbright = Instance.new("TextButton")
local UICorner = Instance.new("UICorner")
local UICorner2 = Instance.new("UICorner")
--local UIGradient = Instance.new("UIGradient")
local InfiniteJump = Instance.new("TextButton")
local Speed = Instance.new("TextButton")
local HomeBtn = Instance.new("TextButton")
local scriptBtn = Instance.new("TextButton")
local Open = Instance.new("ImageButton")
local Home = Instance.new("ImageButton")
local build = Instance.new("ImageButton")
local ScriptHub = Instance.new("ImageButton")
local TextBox = Instance.new("TextBox")
local SoundClick = Instance.new("Sound")
local SoundClick2 = Instance.new("Sound")
--Value:
local Autofram = false
local clickedtime  = 1
local OpenMain = false
--Properties:

--ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.Parent = game.CoreGui

SoundClick.SoundId = "rbxassetid://4572226779"
SoundClick.Parent = ScreenGui
SoundClick2.SoundId = "rbxassetid://4572227011"
SoundClick2.Parent = ScreenGui

TextLabell.BackgroundTransparency = 1
TextLabell.Position = UDim2.new(0.078, 0,0.164, 0)
TextLabell.Size = UDim2.new(0, 146,0, 35)
TextLabell.Font = Enum.Font.SourceSans
TextLabell.Text = "•  New BadTime Hub UI!"
TextLabell.TextSize = 20
TextLabell.TextStrokeTransparency = 1
TextLabell.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabell.Parent = Dash
TextLabell.AutoLocalize = true

Namee.BackgroundTransparency = 1
Namee.Position = UDim2.new(0.082, 0,0.059, 0)
Namee.Size = UDim2.new(0, 141,0, 31)
Namee.Font = Enum.Font.SourceSans
Namee.Text = "• Changelog v.1.1"
Namee.TextSize = 14
Namee.TextStrokeTransparency = 1
Namee.TextColor3 = Color3.fromRGB(106, 106, 106)
Namee.Parent = Dash
Namee.AutoLocalize = true

Eth.BackgroundTransparency = 1
Eth.Position = UDim2.new(0.098, 0,0.018, 0)
Eth.Size = UDim2.new(0, 141,0, 31)
Eth.Font = Enum.Font.SourceSansBold
Eth.Text = "B A D T I M E"
Eth.TextSize = 19
Eth.TextStrokeTransparency = 1
Eth.TextColor3 = Color3.fromRGB(255, 255, 255)
Eth.Parent = Dash
Eth.AutoLocalize = true

Frame.Size = UDim2.new(0, 442,0, 1)
Frame.Position = UDim2.new(0.038, 0,0.145, 0)
Frame.Parent = Dash
Frame.AutoLocalize = true
Frame.Active = false
Frame.BorderSizePixel = 0
Frame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)

scriptFrame.Name = "ScriptFrame"
scriptFrame.Size = UDim2.new(0, 498,0, 399)
scriptFrame.Position = UDim2.new(0.202, 0,1, 0)
scriptFrame.Parent = Main
scriptFrame.Active = false
scriptFrame.BackgroundTransparency = 1
scriptFrame.AutoLocalize = true

Dash.Name = "DashFrame"
Dash.Size = UDim2.new(0, 498,0, 399)
Dash.Position = UDim2.new(0.202, 0,0.098, 0)
Dash.Parent = Main
Dash.Active = false
Dash.BackgroundTransparency = 1
Dash.AutoLocalize = true

DT.BackgroundTransparency = 1
DT.Position = UDim2.new(0.357, 0,0.286, 0)
DT.Size = UDim2.new(0, 59,0, 20)
DT.Font = Enum.Font.SourceSans
DT.Text = "Dashboard"
DT.TextSize = 14
DT.TextStrokeTransparency = 1
DT.TextColor3 = Color3.fromRGB(255, 255, 255)
DT.Parent = Side

Navigation.Name = "Navigation"
Navigation.Position = UDim2.new(0, 9,0.293, 0)
Navigation.Size = UDim2.new(0, 1,0, 16)
Navigation.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Navigation.Parent = Side
Navigation.BorderSizePixel = 0
Navigation.AutoLocalize = true

build.Name = "build"
build.Parent = Dash
build.BackgroundTransparency = 1
build.Position = UDim2.new(0.052, 0,0.032, 0)
build.Size = UDim2.new(0, 35,0, 38)
build.Active = true
build.Image = "rbxassetid://3926307971"
build.ScaleType = Enum.ScaleType.Fit
build.ImageRectOffset = Vector2.new(964, 4)
build.ImageRectSize = Vector2.new(36, 36)

HomeBtn.Text = ""
HomeBtn.ZIndex = 4
HomeBtn.BackgroundTransparency = 1
HomeBtn.Size = UDim2.new(0, 94,0, 25)
HomeBtn.Position = UDim2.new(0.153, 0,0.282, 0)
HomeBtn.Selectable = true
HomeBtn.AutoButtonColor = true
HomeBtn.Parent = Side
HomeBtn.MouseButton1Down:connect(function()
	Navigation:TweenPosition(UDim2.new(0, 9,0.293, 0), "Out", "Quint", .9, true)
	Dash:TweenPosition(UDim2.new(0.202, 0,0.098, 0), "Out", "Quint", .9, true)
	scriptFrame:TweenPosition(UDim2.new(0.202, 0,1, 0), "Out", "Quint", .9, true)
end)

Home.Name = "home"
Home.Parent = Side
Home.BackgroundTransparency = 1
Home.Position = UDim2.new(0.159, 0,0.289, 0)
Home.Size = UDim2.new(0, 19,0, 19)
Home.Image = "rbxassetid://3926305904"
Home.ScaleType = Enum.ScaleType.Fit
Home.ImageRectOffset = Vector2.new(964, 204)
Home.ImageRectSize = Vector2.new(36, 36)
Home.ZIndex = 2

SHT.BackgroundTransparency = 1
SHT.Position = UDim2.new(0.347, 0,0.354, 0)
SHT.Size = UDim2.new(0, 59,0, 20)
SHT.Font = Enum.Font.SourceSans
SHT.Text = "Script Hub"
SHT.TextSize = 14
SHT.TextStrokeTransparency = 1
SHT.TextColor3 = Color3.fromRGB(255, 255, 255)
SHT.Parent = Side

scriptBtn.Text = ""
scriptBtn.ZIndex = 4
scriptBtn.BackgroundTransparency = 1
scriptBtn.Size = UDim2.new(0, 94,0, 25)
scriptBtn.Position = UDim2.new(0.153, 0,0.352, 0)
scriptBtn.Selectable = true
scriptBtn.AutoButtonColor = true
scriptBtn.Parent = Side
scriptBtn.MouseButton1Down:connect(function()
	Navigation:TweenPosition(UDim2.new(0, 9,0.36, 0), "Out", "Quint", .9, true)
	scriptFrame:TweenPosition(UDim2.new(0.202, 0,0.098, 0), "Out", "Quint", .9, true)
	Dash:TweenPosition(UDim2.new(0.202, 0,1, 0), "Out", "Quint", .9, true)
end)

ScriptHub.Name = "sort"
ScriptHub.Parent = Side
ScriptHub.BackgroundTransparency = 1
ScriptHub.Position = UDim2.new(0.159, 0,0.359, 0)
ScriptHub.Size = UDim2.new(0, 19,0, 19)
ScriptHub.Image = "rbxassetid://3926307971"
ScriptHub.ScaleType = Enum.ScaleType.Fit
ScriptHub.ImageRectOffset = Vector2.new(404, 44)
ScriptHub.ImageRectSize = Vector2.new(36, 36)
ScriptHub.ZIndex = 2

Side.Name = "SideBar"
Side.Size = UDim2.new(0, 126,0, 443)
Side.Position = UDim2.new(0,0,0,0)
Side.BackgroundColor3 = Color3.fromRGB(27, 27, 27)
Side.Parent = Main
Side.ZIndex = 5

Version.BackgroundTransparency = 1
Version.Position = UDim2.new(0.735, 0,0.911, 0)
Version.Size = UDim2.new(0, 146,0, 35)
Version.Font = Enum.Font.SourceSans
Version.Text = "Changelog v.1.1"
Version.TextSize = 16
Version.TextStrokeTransparency = 1
Version.TextColor3 = Color3.fromRGB(255, 255, 255)
Version.Parent = Dash

ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
UICorner.CornerRadius = UDim.new(0,4)
UICorner.Parent = Main
UICorner2.CornerRadius = UDim.new(0,4)
UICorner2.Parent = Side

Main.Name = "Main"
Main.Parent = ScreenGui
Main.BackgroundColor3 = Color3.fromRGB(25,25,25)
Main.BorderColor3 = Color3.fromRGB(0, 0, 0)
Main.BorderSizePixel = 0
Main.Position = UDim2.new(0.274, 0,1.821, 0)
Main.Size = UDim2.new(0, 624,0, 443)
Main.Active = true
Main.Draggable = true
Main.ClipsDescendants = true

TextBox.Position = UDim2.new(0.069, 0,0.174, 0)
TextBox.Parent = scriptFrame
TextBox.ZIndex = 2
TextBox.Size = UDim2.new(0, 200,0, 50)
TextBox.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextBox.Font = Enum.Font.SourceSansBold
TextBox.TextScaled = true

Logo.BackgroundTransparency = 1
Logo.Position = UDim2.new(0.017, 0,0.029, 0)
Logo.Size = UDim2.new(0.084, 0,0.042, 0)
Logo.Font = Enum.Font.SourceSansBold
Logo.Text = "B A D H U B"
Logo.TextSize = 27
Logo.TextStrokeTransparency = 1
Logo.TextColor3 = Color3.fromRGB(255, 255, 255)
Logo.TextXAlignment = Enum.TextXAlignment.Left
Logo.Parent = Main
Logo.ZIndex = 100

Close.Name = "Close"
Close.Parent = Main
Close.BackgroundTransparency = 1
Close.Position = UDim2.new(0.934, 0,0, 0)
Close.Size = UDim2.new(0, 43,0, 40)
Close.Font = Enum.Font.SourceSans
Close.Text = "×"
Close.TextColor3 = Color3.fromRGB(255, 255, 255)
Close.TextScaled = false
Close.TextSize = 30
Close.TextStrokeTransparency = 0.000
Close.TextWrapped = false
Close.MouseButton1Down:connect(function()
	if OpenMain == true then
		SoundClick:Play()
		Open.Visible = true
		Main:TweenPosition(UDim2.new(0.274, 0,1.821, 0),"Out","Quint",1,true)
	wait(.5)
	OpenMain = false
end
end)

EspName.Name = "Earned All Chest"
EspName.Parent = scriptFrame
EspName.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
EspName.BackgroundTransparency = 0.900
EspName.BorderColor3 = Color3.fromRGB(0, 0, 0)
EspName.BorderSizePixel = 0
EspName.Position = UDim2.new(0.042, 0,0.677, 0)
EspName.Size = UDim2.new(0, 200,0, 50)
EspName.Font = Enum.Font.Arcade
EspName.Text = "Earned All Chest"
EspName.TextColor3 = Color3.fromRGB(255, 255, 255)
EspName.TextScaled = true
EspName.TextSize = 14.000
EspName.TextStrokeTransparency = 0.000
EspName.TextWrapped = true
EspName.MouseButton1Down:connect(function()
	SoundClick2:Play()
	for k,v in pairs(game:GetService("Workspace").Chests:GetChildren()) do 
		firetouchinterest(game.Players.LocalPlayer.Character.HumanoidRootPart,v,0)    
	end
end)

Fullbright.Name = "Autofram"
Fullbright.Parent = scriptFrame
Fullbright.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Fullbright.BackgroundTransparency = 0.900
Fullbright.BorderColor3 = Color3.fromRGB(0, 0, 0)
Fullbright.BorderSizePixel = 0
Fullbright.Position = UDim2.new(0.624, 0,0.172, 0)
Fullbright.Size = UDim2.new(0, 200,0, 50)
Fullbright.Font = Enum.Font.Arcade
Fullbright.Text = "Auto Fram:Off"
Fullbright.TextColor3 = Color3.fromRGB(255, 255, 255)
Fullbright.TextScaled = true
Fullbright.TextSize = 14.000
Fullbright.TextStrokeTransparency = 0.000
Fullbright.TextWrapped = true
Fullbright.MouseButton1Down:connect(function()
	if Autofram == false then
		SoundClick2:Play()
		Fullbright.Text = "Auto Fram:On"
		Autofram = true
	elseif Autofram == true then
		SoundClick2:Play()
	Fullbright.Text = "Auto Fram:Off"
		Autofram = false
	end
end)

InfiniteJump.Name = "InfiniteJump"
InfiniteJump.Parent = scriptFrame
InfiniteJump.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
InfiniteJump.BackgroundTransparency = 0.900
InfiniteJump.BorderColor3 = Color3.fromRGB(0, 0, 0)
InfiniteJump.BorderSizePixel = 0
InfiniteJump.Position = UDim2.new(0.62244463, 0, 0.54112041, 0)
InfiniteJump.Size = UDim2.new(0, 200, 0, 50)
InfiniteJump.Font = Enum.Font.Arcade
InfiniteJump.Text = "Infinite Jump"
InfiniteJump.TextColor3 = Color3.fromRGB(255, 255, 255)
InfiniteJump.TextScaled = true
InfiniteJump.TextSize = 14.000
InfiniteJump.TextStrokeTransparency = 0.000
InfiniteJump.TextWrapped = true
InfiniteJump.MouseButton1Down:connect(function()
	SoundClick2:Play()
	local InfiniteJumpEnabled = true
	game:GetService("UserInputService").JumpRequest:connect(function()
		if InfiniteJumpEnabled then
			game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
		end
	end)
	local InfiniteJump = CreateButton("Infinite Jump: Off", StuffFrame)
	InfiniteJump.Position = UDim2.new(0,10,0,130)
	InfiniteJump.Size = UDim2.new(0,150,0,30)
	InfiniteJump.MouseButton1Click:connect(function()
		local state = InfiniteJump.Text:sub(string.len("Infinite Jump: ") + 1) --too lazy to count lol
		local new = state == "Off" and "On" or state == "On" and "Off"
		InfiniteJumpEnabled = new == "On"
		InfiniteJump.Text = "Infinite Jump: " .. new
	end)
end)

Speed.Name = "Speed"
Speed.Parent = scriptFrame
Speed.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Speed.BackgroundTransparency = 0.900
Speed.BorderColor3 = Color3.fromRGB(0, 0, 0)
Speed.BorderSizePixel = 0
Speed.Position = UDim2.new(0.069, 0,0.327, 0)
Speed.Size = UDim2.new(0, 200,0, 24)
Speed.Font = Enum.Font.Arcade
Speed.Text = "Speed"
Speed.TextColor3 = Color3.fromRGB(255, 255, 255)
Speed.TextScaled = true
Speed.TextSize = 14.000
Speed.TextStrokeTransparency = 0.000
Speed.TextWrapped = true
Speed.MouseButton1Down:connect(function()
	SoundClick2:Play()
	game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = TextBox.Text
end)

Open.Name = "Open"
Open.Parent = ScreenGui
Open.BackgroundTransparency = 1
Open.Position = UDim2.new(0.015, 0,0.445, 0)
Open.Size = UDim2.new(0, 60,0, 32)
Open.Active = true
Open.Image = "rbxassetid://3926307971"
Open.ScaleType = Enum.ScaleType.Fit
Open.ImageRectOffset = Vector2.new(964, 4)
Open.ImageRectSize = Vector2.new(36, 36)

Open.MouseButton1Down:connect(function()
	if OpenMain == false then
		SoundClick:Play()
		Open.Visible = false
		--Main.Visible = true
		Main:TweenPosition(UDim2.new(0.268, 0,0.121, 0),"Out","Quint",1,true)
		wait()
		OpenMain = true
	end
end)
game:GetService("RunService").Heartbeat:Connect(function()
	if Autofram == true then
		if game.Players.LocalPlayer.Backpack:FindFirstChild("Yoru") then
			game.Players.LocalPlayer.Character.Humanoid:EquipTool(game.Players.LocalPlayer.Backpack:FindFirstChild("Katana"))
		end
		for i,v in pairs(game.Workspace:FindFirstChild("Mod"):GetChildren()) do
			if v:FindFirstChild("HumanoidRootPart") then
				task.wait(0.5)
				game.Workspace:WaitForChild(game.Players.LocalPlayer.Name).HumanoidRootPart.CFrame = v:FindFirstChild("HumanoidRootPart").CFrame
			end
		end
		if clickedtime == 1 then
			clickedtime = 2
			game.Players.LocalPlayer.Character:FindFirstChildWhichIsA("Tool").Remotes.RemotePunch:FireServer("Key1",game.Players.LocalPlayer.Character:FindFirstChildWhichIsA("Tool").Handle.Damage)
		elseif clickedtime == 2 then
			clickedtime = 3
			game.Players.LocalPlayer.Character:FindFirstChildWhichIsA("Tool").Remotes.RemotePunch:FireServer("Key2",game.Players.LocalPlayer.Character:FindFirstChildWhichIsA("Tool").Handle.Damage)
		elseif clickedtime == 3 then    
			clickedtime = 3
			game.Players.LocalPlayer.Character:FindFirstChildWhichIsA("Tool").Remotes.RemotePunch:FireServer("Key3",game.Players.LocalPlayer.Character:FindFirstChildWhichIsA("Tool").Handle.Damage)
		end
	end
end)
