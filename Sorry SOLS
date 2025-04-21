local Players = game:GetService("Players")
local player = Players.LocalPlayer

-- GUI
local gui = Instance.new("ScreenGui", player:WaitForChild("PlayerGui"))
gui.Name = "ANS_Luminosity_GUI"
gui.ResetOnSpawn = false

-- شعار ANS
local logo = Instance.new("ImageLabel", gui)
logo.Size = UDim2.new(0, 200, 0, 200)
logo.Position = UDim2.new(0.5, -100, 0.4, 0)
logo.BackgroundTransparency = 1
logo.Image = "rbxassetid://78674954399214" -- شعار ANS

-- يخفي الشعار بعد 3 ثواني
task.delay(3, function()
	logo:Destroy()
end)

-- إطار الزر N
local holder = Instance.new("Frame", gui)
holder.Size = UDim2.new(0, 40, 0, 40)
holder.Position = UDim2.new(0, 10, 0.5, -20)
holder.BackgroundTransparency = 1
holder.Active = true
holder.Draggable = true

-- الزر N
local button = Instance.new("TextButton", holder)
button.Size = UDim2.new(1, 0, 1, 0)
button.Text = "N"
button.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
button.TextColor3 = Color3.fromRGB(255, 255, 255)
button.Font = Enum.Font.GothamBold
button.TextSize = 16
button.BackgroundTransparency = 0
button.AutoButtonColor = true

-- عرض Luminosity
local function showLuminosity()
	local popup = Instance.new("Frame", gui)
	popup.Size = UDim2.new(1, 0, 1, 0)
	popup.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
	popup.BackgroundTransparency = 0.2

	local text = Instance.new("TextLabel", popup)
	text.Size = UDim2.new(1, 0, 0.3, 0)
	text.Position = UDim2.new(0, 0, 0.35, 0)
	text.BackgroundTransparency = 1
	text.Text = "YOU ROLLED: LUMINOSITY"
	text.TextColor3 = Color3.fromRGB(255, 255, 255)
	text.Font = Enum.Font.GothamBlack
	text.TextScaled = true

	local image = Instance.new("ImageLabel", popup)
	image.Size = UDim2.new(0, 200, 0, 200)
	image.Position = UDim2.new(0.5, -100, 0.2, 0)
	image.BackgroundTransparency = 1
	image.Image = "rbxassetid://16086746317" -- Luminosity

	wait(5)
	popup:Destroy()
end

button.MouseButton1Click:Connect(showLuminosity)
