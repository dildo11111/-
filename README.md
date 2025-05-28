-- СКРИПТ СДЕЛАН РУССКИМ КРАКЕНОМ ТИМ

function sandbox(var,func)
	local env = getfenv(func)
	local newenv = setmetatable({},{
		__index = function(self,k)
			if k=="script" then
				return var
			else
				return env[k]
			end
		end,
	})
	setfenv(func,newenv)
	return func
end
cors = {}
mas = Instance.new("Model",game:GetService("Lighting"))
ScreenGui0 = Instance.new("ScreenGui")
Frame1 = Instance.new("Frame")
TextLabel2 = Instance.new("TextLabel")
TextButton3 = Instance.new("TextButton")
LocalScript4 = Instance.new("LocalScript")
TextBox5 = Instance.new("TextBox")
LocalScript6 = Instance.new("LocalScript")
Animation7 = Instance.new("Animation")
ScreenGui0.Name = "Bang"
ScreenGui0.Parent = mas
ScreenGui0.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
Frame1.Name = "bangframe"
Frame1.Parent = ScreenGui0
Frame1.Position = UDim2.new(0.293236285, 0, 0.216049373, 0)
Frame1.Size = UDim2.new(0, 386, 0, 208)
Frame1.BackgroundColor = BrickColor.new("Toothpaste")
Frame1.BackgroundColor3 = Color3.new(0, 1, 1)
Frame1.BorderColor = BrickColor.new("Really black")
Frame1.BorderColor3 = Color3.new(0, 0, 0)
Frame1.BorderSizePixel = 0
TextLabel2.Parent = Frame1
TextLabel2.Position = UDim2.new(-0.00259067351, 0, 0, 0)
TextLabel2.Size = UDim2.new(0, 386, 0, 73)
TextLabel2.BackgroundColor = BrickColor.new("Institutional white")
TextLabel2.BackgroundColor3 = Color3.new(1, 1, 1)
TextLabel2.BackgroundTransparency = 1
TextLabel2.BorderColor = BrickColor.new("Really black")
TextLabel2.BorderColor3 = Color3.new(0, 0, 0)
TextLabel2.BorderSizePixel = 0
TextLabel2.Font = Enum.Font.SourceSans
TextLabel2.FontSize = Enum.FontSize.Size14
TextLabel2.Text = "Секс порно сиськи письки by Kraken team"
TextLabel2.TextColor = BrickColor.new("Really black")
TextLabel2.TextColor3 = Color3.new(0, 0, 0)
TextLabel2.TextScaled = true
TextLabel2.TextSize = 14
TextLabel2.TextWrap = true
TextLabel2.TextWrapped = true
TextButton3.Parent = Frame1
TextButton3.Position = UDim2.new(0.116031468, 0, 0.747977495, 0)
TextButton3.Size = UDim2.new(0, 303, 0, 41)
TextButton3.BackgroundColor = BrickColor.new("Toothpaste")
TextButton3.BackgroundColor3 = Color3.new(0, 1, 0.933333)
TextButton3.BorderColor = BrickColor.new("Really black")
TextButton3.BorderColor3 = Color3.new(0, 0, 0)
TextButton3.BorderSizePixel = 5
TextButton3.Font = Enum.Font.SourceSans
TextButton3.FontSize = Enum.FontSize.Size14
TextButton3.Text = "Погнали ебаться"
TextButton3.TextColor = BrickColor.new("Really black")
TextButton3.TextColor3 = Color3.new(0, 0, 0)
TextButton3.TextScaled = true
TextButton3.TextSize = 14
TextButton3.TextWrap = true
TextButton3.TextWrapped = true
LocalScript4.Parent = TextButton3
table.insert(cors,sandbox(LocalScript4,function()
button=script.Parent
textbox=button.Parent.TextBox
local lclplr=game.Players.LocalPlayer
local char=lclplr.Character
local banganim = char:WaitForChild("Humanoid"):LoadAnimation(button.Parent.Animation)
bang=false
local function Rape()
	local nickname=textbox.Text
	local victim=workspace:FindFirstChild(nickname)
	if victim and victim:FindFirstChild("HumanoidRootPart") then
		bang=true
		local victimHRP = victim.HumanoidRootPart
		defspeed=char.Humanoid.WalkSpeed
		char.Humanoid.WalkSpeed=0
		textbox.Text=""
		banganim:Play()
			while bang==true do
				char.HumanoidRootPart.CFrame = victimHRP.CFrame + victimHRP.CFrame.LookVector * -5
				task.wait(0.05)
				char.HumanoidRootPart.CFrame = victimHRP.CFrame + victimHRP.CFrame.LookVector * -3
				task.wait(0.05)
				char.HumanoidRootPart.CFrame = victimHRP.CFrame + victimHRP.CFrame.LookVector * -1
				task.wait(0.05)
				char.HumanoidRootPart.CFrame = victimHRP.CFrame + victimHRP.CFrame.LookVector * -0.7
				task.wait(0.05)
				char.HumanoidRootPart.CFrame = victimHRP.CFrame + victimHRP.CFrame.LookVector * -1
				task.wait(0.05)
				char.HumanoidRootPart.CFrame = victimHRP.CFrame + victimHRP.CFrame.LookVector * -3
				task.wait(0.05)
			end
			else
				bang=false
				char.Humanoid.WalkSpeed=defspeed
				banganim:Stop()
	end
end
button.MouseButton1Click:Connect(Rape)

end))
TextBox5.Parent = Frame1
TextBox5.Position = UDim2.new(0.238341972, 0, 0.379807681, 0)
TextBox5.Size = UDim2.new(0, 200, 0, 50)
TextBox5.BackgroundColor = BrickColor.new("Institutional white")
TextBox5.BackgroundColor3 = Color3.new(1, 1, 1)
TextBox5.BorderColor = BrickColor.new("Really black")
TextBox5.BorderColor3 = Color3.new(0, 0, 0)
TextBox5.BorderSizePixel = 0
TextBox5.Font = Enum.Font.SourceSans
TextBox5.FontSize = Enum.FontSize.Size14
TextBox5.Text = ""
TextBox5.TextColor = BrickColor.new("Really black")
TextBox5.TextColor3 = Color3.new(0, 0, 0)
TextBox5.TextScaled = true
TextBox5.TextSize = 14
TextBox5.TextWrap = true
TextBox5.TextWrapped = true
TextBox5.ClearTextOnFocus = false
TextBox5.PlaceholderColor3 = Color3.new(0, 0, 0)
TextBox5.PlaceholderText = "Кого ебать будем?"
LocalScript6.Name = "UIDrag"
LocalScript6.Parent = Frame1
table.insert(cors,sandbox(LocalScript6,function()
-- Made by Real_IceyDev (@lceyDex) --
-- Simple UI dragger (PC Only/Any device that has a mouse) --

local UIS = game:GetService('UserInputService')
local frame = script.Parent
local dragToggle = nil
local dragSpeed = 0.25
local dragStart = nil
local startPos = nil

local function updateInput(input)
	local delta = input.Position - dragStart
	local position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X,
		startPos.Y.Scale, startPos.Y.Offset + delta.Y)
	game:GetService('TweenService'):Create(frame, TweenInfo.new(dragSpeed), {Position = position}):Play()
end

frame.InputBegan:Connect(function(input)
	if (input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch) then 
		dragToggle = true
		dragStart = input.Position
		startPos = frame.Position
		input.Changed:Connect(function()
			if input.UserInputState == Enum.UserInputState.End then
				dragToggle = false
			end
		end)
	end
end)

UIS.InputChanged:Connect(function(input)
	if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
		if dragToggle then
			updateInput(input)
		end
	end
end)
end))
Animation7.Parent = Frame1
Animation7.AnimationId = "rbxassetid://106772613"
for i,v in pairs(mas:GetChildren()) do
	v.Parent = game:GetService("Players").LocalPlayer.PlayerGui
	pcall(function() v:MakeJoints() end)
end
mas:Destroy()
for i,v in pairs(cors) do
	spawn(function()
		pcall(v)
	end)
end
