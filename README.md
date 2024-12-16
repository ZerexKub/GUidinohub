-- UI Credits to fluke

local DINOHUB = Instance.new("ScreenGui")
local OPENCLOSE = Instance.new("TextButton")


DINOHUB.Name = "fluke Hub"
DINOHUB.Parent = game.CoreGui
DINOHUB.ZIndexBehavior = Enum.ZIndexBehavior.Sibling


OPENCLOSE.Name = "OPENCLOSE"
OPENCLOSE.Parent = DINOHUB
OPENCLOSE.BackgroundColor3 = Color3.fromRGB(153, 153, 153)
OPENCLOSE.BorderSizePixel = 0
OPENCLOSE.Position = UDim2.new(0.186344236, 0, 0.239436626, 0)
OPENCLOSE.Size = UDim2.new(0, 56, 0, 31)
OPENCLOSE.Font = Enum.Font.DenkOne
OPENCLOSE.Text = "ZX HUB"
OPENCLOSE.TextColor3 = Color3.fromRGB(255, 255, 255)
OPENCLOSE.TextScaled = true
OPENCLOSE.TextSize = 14.000
OPENCLOSE.TextWrapped = true
OPENCLOSE.MouseButton1Click:Connect(function()
    game.CoreGui:FindFirstChild("DinoUI").Enabled = not game.CoreGui:FindFirstChild("DinoUI").Enabled
end)
do
   if game:GetService("CoreGui"):FindFirstChild("DinoUI") then
      game:GetService("CoreGui").DinoUI:Destroy()
  -- UI Credits to Sanda

local DINOHUB = Instance.new("ScreenGui")
local OPENCLOSE = Instance.new("TextButton")


DINOHUB.Name = "zerex hub"
DINOHUB.Parent = game.CoreGui
DINOHUB.ZIndexBehavior = Enum.ZIndexBehavior.Sibling


OPENCLOSE.Name = "OPENCLOSE"
OPENCLOSE.Parent = DINOHUB
OPENCLOSE.BackgroundColor3 = Color3.fromRGB(153, 153, 153)
OPENCLOSE.BorderSizePixel = 0
OPENCLOSE.Position = UDim2.new(0.186344236, 0, 0.239436626, 0)
OPENCLOSE.Size = UDim2.new(0, 56, 0, 31)
OPENCLOSE.Font = Enum.Font.DenkOne
OPENCLOSE.Text = "PDHUB"
OPENCLOSE.TextColor3 = Color3.fromRGB(255, 255, 255)
OPENCLOSE.TextScaled = true
OPENCLOSE.TextSize = 14.000
OPENCLOSE.TextWrapped = true
OPENCLOSE.MouseButton1Click:Connect(function()
    game.CoreGui:FindFirstChild("DinoUI").Enabled = not game.CoreGui:FindFirstChild("DinoUI").Enabled
end)
do
   if game:GetService("CoreGui"):FindFirstChild("DinoUI") then
      game:GetService("CoreGui").DinoUI:Destroy()
  end
end
local TweenService = game:GetService("TweenService")
local UserInputService = game:GetService("UserInputService")
local Dino = {}
game:GetService("UserInputService").InputBegan:Connect(function(key)
if key.KeyCode == Enum.KeyCode.RightControl then
   game.CoreGui:FindFirstChild("DinoUI").Enabled = not game.CoreGui:FindFirstChild("DinoUI").Enabled
end
end)
game:GetService("UserInputService").InputBegan:Connect(function(key)
if key.KeyCode == Enum.KeyCode.RightControl then
   game:GetService("CoreGui").DINOHUB.Enabled = not game:GetService("CoreGui").DINOHUB.Enabled
end
end)
function Dino:CreateWindow(dinotitle)
   local DinoUI = Instance.new("ScreenGui")
   local Window = Instance.new("Frame")
   local DinoHubText1 = Instance.new("TextLabel")
   local DinoHubText2 = Instance.new("TextLabel")
   local WindowText = Instance.new("TextLabel")
   local TabWindow = Instance.new("ScrollingFrame")
   local TabWindowList = Instance.new("UIListLayout")
   local ContainerHolder = Instance.new("Frame")

   --Properties:

   DinoUI.Name = "DinoUI"
   DinoUI.Parent = game.CoreGui
   DinoUI.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

   Window.Name = "Window"
   Window.Parent = DinoUI
   Window.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
   Window.BorderSizePixel = 0
   Window.Position = UDim2.new(0, 392, 0, 264)
   Window.Size = UDim2.new(0, 390, 0, 350)

   DinoHubText1.Name = "DinoHubText1"
   DinoHubText1.Parent = Window
   DinoHubText1.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
   DinoHubText1.BackgroundTransparency = 1.000
   DinoHubText1.BorderSizePixel = 0
   DinoHubText1.Position = UDim2.new(0, 5, 0, 0)
   DinoHubText1.Size = UDim2.new(0, 35, 0, 20)
   DinoHubText1.Font = Enum.Font.GothamSemibold
   DinoHubText1.Text = " zerex"
   DinoHubText1.TextColor3 = Color3.fromRGB(180, 180, 180)
   DinoHubText1.TextSize = 13.000

   DinoHubText2.Name = "DinoHubText2"
   DinoHubText2.Parent = Window
   DinoHubText2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
   DinoHubText2.BackgroundTransparency = 1.000
   DinoHubText2.BorderSizePixel = 0
   DinoHubText2.Position = UDim2.new(0, 40, 0, 0)
   DinoHubText2.Size = UDim2.new(0, 35, 0, 20)
   DinoHubText2.Font = Enum.Font.GothamSemibold
   DinoHubText2.Text = "          Hub   |  "
   DinoHubText2.TextColor3 = Color3.fromRGB(144, 255, 255)
   DinoHubText2.TextSize = 13.000

   WindowText.Name = "WindowText"
   WindowText.Parent = Window
   WindowText.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
   WindowText.BackgroundTransparency = 1.000
   WindowText.BorderSizePixel = 0
   WindowText.Position = UDim2.new(0, 85, 0, 0)
   WindowText.Size = UDim2.new(0, 305, 0, 20)
   WindowText.Font = Enum.Font.GothamSemibold
   WindowText.Text = dinotitle or "Game Title"
   WindowText.TextColor3 = Color3.fromRGB(150, 150, 150)
   WindowText.TextSize = 13.000
   WindowText.TextXAlignment = Enum.TextXAlignment.Left

   TabWindow.Name = "TabWindow"
   TabWindow.Parent = Window
   TabWindow.Active = true
   TabWindow.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
   TabWindow.BorderSizePixel = 0
   TabWindow.Position = UDim2.new(0, 7, 0, 20)
   TabWindow.Size = UDim2.new(0, 375, 0, 20)
   TabWindow.CanvasSize = UDim2.new(2, 0, 0, 0)
   TabWindow.ScrollBarThickness = 2

   TabWindowList.Name = "TabWindowList"
   TabWindowList.Parent = TabWindow
   TabWindowList.FillDirection = Enum.FillDirection.Horizontal
   TabWindowList.SortOrder = Enum.SortOrder.LayoutOrder

   ContainerHolder.Name = "ContainerHolder"
   ContainerHolder.Parent = Window
   ContainerHolder.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
   ContainerHolder.BorderSizePixel = 0
   ContainerHolder.Position = UDim2.new(0, 0, 0, 40)
   ContainerHolder.Size = UDim2.new(0, 390, 0, 310)

   -- Don't Touch This Script Or It Will Mess Up --

   TabWindow.CanvasSize = UDim2.new(0, 0 + TabWindowList.AbsoluteContentSize.X, 0, 0)
   TabWindowList:GetPropertyChangedSignal("AbsoluteContentSize"):Connect(function()
   TabWindow.CanvasSize = UDim2.new(0, 0 + TabWindowList.AbsoluteContentSize.X, 0, 0)
   end)

   local gui = Window

   local dragging
   local dragInput
   local dragStart
   local startPos

   local function update(input)
      local delta = input.Position - dragStart
      gui.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
   end

   gui.InputBegan:Connect(function(input)
   if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
      dragging = true
      dragStart = input.Position
      startPos = gui.Position

      input.Changed:Connect(function()
      if input.UserInputState == Enum.UserInputState.End then
         dragging = false
      end
      end)
   end
   end)

   gui.InputChanged:Connect(function(input)
   if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
      dragInput = input
   end
   end)

   UserInputService.InputChanged:Connect(function(input)
   if input == dragInput and dragging then
      update(input)
   end
   end)

   local DinoWindow = {}

   function DinoWindow:NewPage(pagetitle)
      local Container = Instance.new("ScrollingFrame")
      local ContainerList = Instance.new("UIListLayout")

      --Properties:

      Container.Name = pagetitle or "Container"
      Container.Parent = ContainerHolder
      Container.Active = true
      Container.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
      Container.BorderSizePixel = 0
      Container.Position = UDim2.new(0, 5, 0, 5)
      Container.Size = UDim2.new(0, 380, 0, 300)
      Container.Visible = false
      Container.CanvasSize = UDim2.new(0, 0, 0, 5 + ContainerList.Padding.Offset + ContainerList.AbsoluteContentSize.Y)
      Container.ScrollBarThickness = 2

      ContainerList.Name = "ContainerList"
      ContainerList.Parent = Container
      ContainerList.HorizontalAlignment = Enum.HorizontalAlignment.Center
      ContainerList.SortOrder = Enum.SortOrder.LayoutOrder
      ContainerList.Padding = UDim.new(0, 5)

      -- Don't Touch This Script Or It Will Mess Up --
      ContainerList:GetPropertyChangedSignal("AbsoluteContentSize"):Connect(function()
      Container.CanvasSize = UDim2.new(0, 0, 0, 0 + ContainerList.Padding.Offset + ContainerList.AbsoluteContentSize.Y)
      end)

      Container.ChildAdded:Connect(function()
      Container.CanvasSize = UDim2.new(0, 0, 0, 0 + ContainerList.Padding.Offset + ContainerList.AbsoluteContentSize.Y)
      end)

      local TabButton = Instance.new("TextButton")

      --Properties:

      TabButton.Name = "TabButton"
      TabButton.Parent = TabWindow
      TabButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
      TabButton.BackgroundTransparency = 1.000
      TabButton.BorderSizePixel = 0
      TabButton.Position = UDim2.new(0, 5, 0, 0)
      TabButton.Size = UDim2.new(0, 100, 0, 20)
      TabButton.Font = Enum.Font.GothamSemibold
      TabButton.Text = pagetitle or "Tab"
      TabButton.TextColor3 = Color3.fromRGB(180, 180, 180)
      TabButton.TextSize = 13.000

      -- Don't Touch This Script Or It Will Mess Up --

      TabButton.Size = UDim2.new(0, 10 + TabButton.TextBounds.X, 0, 20)

      TabButton.MouseButton1Click:Connect(function()
      for _, co in pairs(ContainerHolder:GetChildren()) do
         if co:IsA("ScrollingFrame") then
            co.Visible = false
         end
      end
      for _, tb in pairs(TabWindow:GetChildren()) do
         if tb:IsA("TextButton") then
            TweenService:Create(tb, TweenInfo.new(0.12, Enum.EasingStyle.Linear, Enum.EasingDirection.InOut), {TextColor3 = Color3.fromRGB(180, 180, 180)}):Play()
         end
      end
      TweenService:Create(TabButton, TweenInfo.new(0.12, Enum.EasingStyle.Linear, Enum.EasingDirection.InOut), {TextColor3 = Color3.fromRGB(125, 125, 125)}):Play()
      Container.Visible = true
      end)

      local DinoPage = {}

      function DinoPage:NewSection(sectiontitle)
         local Section = Instance.new("Frame")
         local SectionTitle = Instance.new("TextLabel")
         local SectionIn = Instance.new("Frame")
         local SectionInUICorner = Instance.new("UICorner")
         local SectionInList = Instance.new("UIListLayout")

         --Properties:

         Section.Name = sectiontitle or "Section"
         Section.Parent = Container
         Section.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
         Section.Position = UDim2.new(0.0263157897, 0, 0, 0)
         Section.Size = UDim2.new(0, 360, 0, 20)

         SectionTitle.Name = "SectionTitle"
         SectionTitle.Parent = Section
         SectionTitle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         SectionTitle.BackgroundTransparency = 1.000
         SectionTitle.BorderSizePixel = 0
         SectionTitle.Size = UDim2.new(0, 360, 0, 15)
         SectionTitle.Font = Enum.Font.GothamSemibold
         SectionTitle.Text = sectiontitle or "Section"
         SectionTitle.TextColor3 = Color3.fromRGB(180, 180, 180)
         SectionTitle.TextSize = 13.000

         SectionIn.Name = "SectionIn"
         SectionIn.Parent = Section
         SectionIn.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
         SectionIn.BorderSizePixel = 0
         SectionIn.Position = UDim2.new(0, 0, 0, 20)
         SectionIn.Size = UDim2.new(0, 360, 0, 70)

         SectionInUICorner.CornerRadius = UDim.new(0, 2)
         SectionInUICorner.Name = "SectionInUICorner"
         SectionInUICorner.Parent = SectionIn

         SectionInList.Name = "SectionInList"
         SectionInList.Parent = SectionIn
         SectionInList.HorizontalAlignment = Enum.HorizontalAlignment.Center
         SectionInList.SortOrder = Enum.SortOrder.LayoutOrder
         SectionInList.Padding = UDim.new(0, 10)

         -- Don't Touch This Script Or It Will Mess Up --

         SectionIn.Size = UDim2.new(0, 360, 0, 5 + SectionInList.AbsoluteContentSize.Y + SectionInList.Padding.Offset)
         SectionInList:GetPropertyChangedSignal("AbsoluteContentSize"):Connect(function()
         SectionIn.Size = UDim2.new(0, 360, 0, 5 + SectionInList.AbsoluteContentSize.Y + SectionInList.Padding.Offset)
         end)

         local function ContainerSizeChange()
            local largestListSize = 0
            largestListSize = SectionInList.AbsoluteContentSize.Y

            Container.CanvasSize = UDim2.new(0, 0, 0, largestListSize + 35 + SectionInList.Padding.Offset)
         end
         local function sectionsizechange()
            Section.Size = UDim2.new(0, 360, 0, 20 + SectionInList.AbsoluteContentSize.Y + SectionInList.Padding.Offset)
         end
         ContainerSizeChange()
         sectionsizechange()

         SectionInList:GetPropertyChangedSignal("AbsoluteContentSize"):Connect(function()
         ContainerSizeChange()
         sectionsizechange()
         end)

         local DinoElement = {}

         function DinoElement:CreateButton(buttontitle, buttoncallback)
            local ButtonHolder = Instance.new("TextButton")
            local ButtonHolderUICorner = Instance.new("UICorner")
            local ButtonHolderUIStroke = Instance.new("UIStroke")
            local ButtonImage = Instance.new("ImageLabel")

            ButtonHolder.Name = buttontitle or "ButtonHolder"
            ButtonHolder.Parent = SectionIn
            ButtonHolder.BackgroundColor3 = Color3.fromRGB(144, 255, 255)
            ButtonHolder.BorderSizePixel = 0
            ButtonHolder.Position = UDim2.new(0, 5, 0, 0)
            ButtonHolder.Size = UDim2.new(0, 350, 0, 25)
            ButtonHolder.AutoButtonColor = false
            ButtonHolder.Font = Enum.Font.GothamSemibold
            ButtonHolder.Text = buttontitle or "Button | Click Me"
            ButtonHolder.TextColor3 = Color3.fromRGB(180, 180, 180)
            ButtonHolder.TextSize = 13.000

            ButtonHolderUICorner.CornerRadius = UDim.new(0, 4)
            ButtonHolderUICorner.Name = "ButtonHolderUICorner"
            ButtonHolderUICorner.Parent = ButtonHolder

            ButtonHolderUIStroke.Name = "ButtonHolderUIStroke"
            ButtonHolderUIStroke.Parent = ButtonHolder
            ButtonHolderUIStroke.ApplyStrokeMode = Enum.ApplyStrokeMode.Border
            ButtonHolderUIStroke.Color = Color3.fromRGB(144, 255, 255)
            ButtonHolderUIStroke.LineJoinMode = Enum.LineJoinMode.Round
            ButtonHolderUIStroke.Thickness = 1.6
            ButtonHolderUIStroke.Transparency = 0
            ButtonHolderUIStroke.Enabled = true
            ButtonHolderUIStroke.Archivable = true

            ButtonImage.Name = "ButtonImage"
            ButtonImage.Parent = ButtonHolder
            ButtonImage.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
            ButtonImage.BackgroundTransparency = 1.000
            ButtonImage.BorderSizePixel = 0
            ButtonImage.Position = UDim2.new(0, 5, 0, 3)
            ButtonImage.Size = UDim2.new(0, 18, 0, 18)
            ButtonImage.Image = "rbxassetid://7839505809"
            ButtonImage.ImageColor3 = Color3.fromRGB(180, 180, 180)

            -- Don't Touch This Script Or It Will Mess Up --

            ButtonHolder.MouseEnter:Connect(function()
            TweenService:Create(ButtonHolder, TweenInfo.new(0.12, Enum.EasingStyle.Linear, Enum.EasingDirection.InOut), {TextColor3 = Color3.fromRGB(125, 125, 125)}):Play()
            TweenService:Create(ButtonImage, TweenInfo.new(0.12, Enum.EasingStyle.Linear, Enum.EasingDirection.InOut), {ImageColor3 = Color3.fromRGB(125, 125, 125)}):Play()
            end)
            ButtonHolder.MouseLeave:Connect(function()
            TweenService:Create(ButtonHolder, TweenInfo.new(0.12, Enum.EasingStyle.Linear, Enum.EasingDirection.InOut), {TextColor3 = Color3.fromRGB(180, 180, 180)}):Play()
            TweenService:Create(ButtonImage, TweenInfo.new(0.12, Enum.EasingStyle.Linear, Enum.EasingDirection.InOut), {ImageColor3 = Color3.fromRGB(180, 180, 180)}):Play()
            TweenService:Create(ButtonHolder, TweenInfo.new(0.12, Enum.EasingStyle.Linear, Enum.EasingDirection.InOut), {Size = UDim2.new(0, 350, 0, 25)}):Play()
            end)
            ButtonHolder.MouseButton1Down:Connect(function()
            TweenService:Create(ButtonHolder, TweenInfo.new(0.12, Enum.EasingStyle.Linear, Enum.EasingDirection.InOut), {Size = UDim2.new(0, 345, 0, 23)}):Play()
            end)
            ButtonHolder.MouseButton1Up:Connect(function()
            TweenService:Create(ButtonHolder, TweenInfo.new(0.12, Enum.EasingStyle.Linear, Enum.EasingDirection.InOut), {Size = UDim2.new(0, 350, 0, 25)}):Play()
            end)
            ButtonHolder.MouseButton1Click:Connect(function()
            pcall(function()
            buttoncallback()
            end)
            end)

         end

         function DinoElement:CreateToggle(toggletitle, togglecallback)
            local ToggleHolder = Instance.new("Frame")
            local ToggleHolderUICorner = Instance.new("UICorner")
            local ToggleImage = Instance.new("ImageLabel")
            local ToggleTitle = Instance.new("TextLabel")
            local ToggleOut = Instance.new("ImageLabel")
            local ToggleOutUICorner = Instance.new("UICorner")
            local ToggleIn = Instance.new("ImageLabel")
            local ToggleInUICorner = Instance.new("UICorner")
            local ToggleHolderButton = Instance.new("TextButton")
            local ToggleHolderUIStroke = Instance.new("UIStroke")

            --Properties:

            ToggleHolder.Name = toggletitle or "ToggleHolder"
            ToggleHolder.Parent = SectionIn
            ToggleHolder.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
            ToggleHolder.BorderSizePixel = 0
            ToggleHolder.Size = UDim2.new(0, 350, 0, 25)

            ToggleHolderUICorner.CornerRadius = UDim.new(0, 1)
            ToggleHolderUICorner.Name = "ToggleHolderUICorner"
            ToggleHolderUICorner.Parent = ToggleHolder

            ToggleImage.Name = "ToggleImage"
            ToggleImage.Parent = ToggleHolder
            ToggleImage.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
            ToggleImage.BackgroundTransparency = 1.000
            ToggleImage.BorderSizePixel = 0
            ToggleImage.Position = UDim2.new(0, 5, 0, 3)
            ToggleImage.Size = UDim2.new(0, 18, 0, 18)
            ToggleImage.Image = "rbxassetid://7832083744"
            ToggleImage.ImageColor3 = Color3.fromRGB(200, 200, 200)

            ToggleTitle.Name = "ToggleTitle"
            ToggleTitle.Parent = ToggleHolder
            ToggleTitle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
            ToggleTitle.BackgroundTransparency = 1.000
            ToggleTitle.BorderSizePixel = 0
            ToggleTitle.Position = UDim2.new(0, 25, 0, 0)
            ToggleTitle.Size = UDim2.new(0, 250, 0, 25)
            ToggleTitle.Font = Enum.Font.GothamSemibold
            ToggleTitle.Text = toggletitle or "Toggle | Toggle Me !"
            ToggleTitle.TextColor3 = Color3.fromRGB(180, 180, 180)
            ToggleTitle.TextSize = 13.000
            ToggleTitle.TextXAlignment = Enum.TextXAlignment.Left

            ToggleOut.Name = "ToggleOut"
            ToggleOut.Parent = ToggleHolder
            ToggleOut.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
            ToggleOut.Position = UDim2.new(0, 310, 0, 4)
            ToggleOut.Size = UDim2.new(0, 34, 0, 16)
            ToggleOut.Image = "rbxasset://textures/ui/GuiImagePlaceholder.png"
            ToggleOut.ImageTransparency = 1.000

            ToggleOutUICorner.CornerRadius = UDim.new(0, 1000)
            ToggleOutUICorner.Name = "ToggleOutUICorner"
            ToggleOutUICorner.Parent = ToggleOut

            ToggleIn.Name = "ToggleIn"
            ToggleIn.Parent = ToggleOut
            ToggleIn.BackgroundColor3 = Color3.fromRGB(144, 255, 255)
            ToggleIn.Position = UDim2.new(0, 2, 0, 2)
            ToggleIn.Size = UDim2.new(0, 12, 0, 12)
            ToggleIn.Image = "rbxasset://textures/ui/GuiImagePlaceholder.png"
            ToggleIn.ImageTransparency = 1.000

            ToggleInUICor
