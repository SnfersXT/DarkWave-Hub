--services
local players = game:GetService("Players")
local tweenService = game:GetService("TweenService")
local runService = game:GetService("RunService")
local StarterGui = game:GetService("StarterGui")
local coreGui = game:GetService("CoreGui")
local uis = game:GetService("UserInputService")
local ts = game:GetService("TweenService")
local TweenService = game:GetService("TweenService")


--vars
local viewport = workspace.CurrentCamera.ViewportSize
local tweenInfo = TweenInfo.new(0.2, Enum.EasingStyle.Quad, Enum.EasingDirection.InOut)

--Script

function CreateWindow(options)

	local GUI = {
		CurrentTab = nil
	}
	local LoaderOptions = options
	--Main Frame
	do
		-- StarterGui.NewMenu
		GUI["1"] = Instance.new("ScreenGui", game:GetService("Players").LocalPlayer:WaitForChild("PlayerGui"));
		GUI["1"]["Name"] = options.Name;
		GUI["1"]["ZIndexBehavior"] = Enum.ZIndexBehavior.Sibling;


		-- StarterGui.NewMenu.Main
		GUI["2"] = Instance.new("Frame", GUI["1"]);
		GUI["2"]["Visible"] = false;
		GUI["2"]["BorderSizePixel"] = 0;
		GUI["2"]["BackgroundColor3"] = Color3.fromRGB(27, 27, 27);
		GUI["2"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		GUI["2"]["Size"] = UDim2.new(0, 600, 0, 375);
		GUI["2"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);
		GUI["2"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["2"]["Name"] = [[Main]];
		GUI["2"]["ClipsDescendants"] = true
		GUI["2"]["BackgroundTransparency"] = 0.05

		-- StarterGui.NewMenu.Main.UICorner
		GUI["3"] = Instance.new("UICorner", GUI["2"]);



		-- StarterGui.NewMenu.Main.TopFrame
		GUI["4"] = Instance.new("Frame", GUI["2"]);
		GUI["4"]["BorderSizePixel"] = 0;
		GUI["4"]["BackgroundColor3"] = Color3.fromRGB(26, 26, 26);
		GUI["4"]["Size"] = UDim2.new(0, 592, 0, 25);
		GUI["4"]["Position"] = UDim2.new(0, 2, 0, 5);
		GUI["4"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["4"]["Name"] = [[TopFrame]];
		GUI["4"]["BackgroundTransparency"] = 1
		
		-- StarterTools.NewMenu.Main.Container.TestTab.Tools.ScrollStart.Items.Tool.UICorner
		GUI["e4"] = Instance.new("UICorner", GUI["4"]);


		-- StarterGui.NewMenu.Main.TopFrame.UIStroke
		GUI["5"] = Instance.new("UIStroke", GUI["4"]);
		GUI["5"]["Color"] = Color3.fromRGB(30, 30, 30);


		-- StarterGui.NewMenu.Main.TopFrame.NameText
		GUI["9"] = Instance.new("TextLabel", GUI["4"]);
		GUI["9"]["TextWrapped"] = true;
		GUI["9"]["BorderSizePixel"] = 0;
		GUI["9"]["TextSize"] = 100;
		GUI["9"]["TextScaled"] = true;
		GUI["9"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["9"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		GUI["9"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["9"]["BackgroundTransparency"] = 1;
		GUI["9"]["Size"] = UDim2.new(0, 125, 0, 32);
		GUI["9"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["9"]["Text"] = options.Name;
		GUI["9"]["Name"] = [[NameText]];
		GUI["9"]["Position"] = UDim2.new(0, 5, -0.2, 0);


		GUI["9"].Font = Enum.Font.GothamSemibold



		-- StarterGui.NewMenu.Main.TopFrame.Close
		GUI["b"] = Instance.new("ImageButton", GUI["4"]);
		GUI["b"]["Active"] = false;
		GUI["b"]["BorderSizePixel"] = 0;
		GUI["b"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["b"]["Selectable"] = false;
		GUI["b"]["Size"] = UDim2.new(0, 30, 0, 30);
		GUI["b"]["BackgroundTransparency"] = 1;
		GUI["b"]["Name"] = [[Close]];
		GUI["b"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["b"]["Image"] = "rbxassetid://10747384394"
		GUI["b"]["Position"] = UDim2.new(0.93, 5, -0.12, 0);




		-- StarterGui.NewMenu.Main.TopFrame.Minimize
		GUI["b1"] = Instance.new("ImageButton", GUI["4"]);
		GUI["b1"]["Active"] = false;
		GUI["b1"]["BorderSizePixel"] = 0;
		GUI["b1"]["Selectable"] = false;
		GUI["b1"]["Size"] = UDim2.new(0, 30, 0, 30);
		GUI["b1"]["BackgroundTransparency"] = 1;
		GUI["b1"]["Name"] = [[Minimize]];
		GUI["b1"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["b1"]["Image"] = "rbxassetid://10734896206"
		GUI["b1"]["Position"] = UDim2.new(0.88, 5, -0.12, 0);
		
		
		
		-- StarterGui.NewMenu.Main.TopFrame.Open
		GUI["b2"] = Instance.new("ImageButton", GUI["4"]);
		GUI["b2"]["Active"] = false;
		GUI["b2"]["Visible"] = false;
		GUI["b2"]["BorderSizePixel"] = 0;
		GUI["b2"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["b2"]["Selectable"] = false;
		GUI["b2"]["Size"] = UDim2.new(0, 30, 0, 30);
		GUI["b2"]["BackgroundTransparency"] = 1;
		GUI["b2"]["Name"] = [[Open]];
		GUI["b2"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["b2"]["Image"] = "rbxassetid://10734924532"
		GUI["b2"]["Position"] = UDim2.new(0.88, 5, -0.12, 0);
		
		
		
	end
	
	--Navigation
	do
		-- StarterGui.NewMenu.Main.Navigation
		GUI["c3"] = Instance.new("ScrollingFrame", GUI["2"]);
		GUI["c3"]["BorderSizePixel"] = 0;
		GUI["c3"]["CanvasSize"] = UDim2.new(0, 0, 0, 0);
		GUI["c3"]["TopImage"] = [[rbxassetid://7445543667]];
		GUI["c3"]["MidImage"] = [[rbxassetid://7445543667]];
		GUI["c3"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["c3"]["Name"] = [[Navigation]];
		GUI["c3"]["ScrollBarImageTransparency"] = 1;
		GUI["c3"]["Selectable"] = false;
		GUI["c3"]["BottomImage"] = [[rbxassetid://7445543667]];
		GUI["c3"]["AutomaticCanvasSize"] = Enum.AutomaticSize.Y;
		GUI["c3"]["Size"] = UDim2.new(0, 100, 0, 335);
		GUI["c3"]["ScrollBarImageColor3"] = Color3.fromRGB(41, 41, 41);
		GUI["c3"]["Position"] = UDim2.new(0, 3, 0, 35);
		GUI["c3"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["c3"]["ScrollBarThickness"] = 4;
		GUI["c3"]["BackgroundTransparency"] = 1;


		-- StarterGui.NewMenu.Main.Navigation.UIStroke
		GUI["c4"] = Instance.new("UIStroke", GUI["c3"]);
		GUI["c4"]["Color"] = Color3.fromRGB(31, 31, 31);


		-- StarterGui.NewMenu.Main.Navigation.UICorner
		GUI["c5"] = Instance.new("UICorner", GUI["c3"]);



		-- StarterGui.NewMenu.Main.Navigation.UIListLayout
		GUI["c6"] = Instance.new("UIListLayout", GUI["c3"]);
		GUI["c6"]["Padding"] = UDim.new(0, 5);
		GUI["c6"]["SortOrder"] = Enum.SortOrder.LayoutOrder;


		-- StarterGui.NewMenu.Main.Navigation.UIPadding
		GUI["c7"] = Instance.new("UIPadding", GUI["c3"]);
		GUI["c7"]["PaddingTop"] = UDim.new(0, 3);
		GUI["c7"]["PaddingLeft"] = UDim.new(0, 1);
		
		


	end

	--Container
	do
		-- StarterGui.NewMenu.Main.Container
		GUI["10"] = Instance.new("Frame", GUI["2"]);
		GUI["10"]["BorderSizePixel"] = 0;
		GUI["10"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["10"]["Size"] = UDim2.new(0, 485, 0, 335);
		GUI["10"]["Position"] = UDim2.new(0, 110, 0, 35);
		GUI["10"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["10"]["Name"] = [[Container]];
		GUI["10"]["BackgroundTransparency"] = 1;


		-- StarterGui.NewMenu.Main.Container.UIStroke
		GUI["11"] = Instance.new("UIStroke", GUI["10"]);
		GUI["11"]["Color"] = Color3.fromRGB(31, 31, 31);


		-- StarterGui.NewMenu.Main.Container.UICorner
		GUI["12"] = Instance.new("UICorner", GUI["10"]);
		
	end
	
	
	if options.LoaderEnabled == true and options.LoadedMain ~= false then
		options.LoadedMain = true
		-- StarterGui.NewMenu.GUI
		GUI["d0"] = Instance.new("Frame", GUI["1"]);
		GUI["d0"]["Visible"] = false;
		GUI["d0"]["BorderSizePixel"] = 0;
		GUI["d0"]["BackgroundColor3"] = Color3.fromRGB(16, 16, 16);
		GUI["d0"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		GUI["d0"]["ClipsDescendants"] = true;
		GUI["d0"]["Size"] = UDim2.new(0, 0, 0, 0);
		GUI["d0"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);
		GUI["d0"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["d0"]["Name"] = [[Loader]];
		GUI["d0"]["Active"] = false;


		-- StarterGui.NewMenu.GUI.UIStroke
		GUI["d1"] = Instance.new("UIStroke", GUI["d0"]);
		GUI["d1"]["Thickness"] = 1.5;
		GUI["d1"]["Color"] = Color3.fromRGB(51, 51, 51);


		-- StarterGui.NewMenu.GUI.UICorner
		GUI["d2"] = Instance.new("UICorner", GUI["d0"]);
		GUI["d2"]["CornerRadius"] = UDim.new(0, 6);


		-- StarterGui.NewMenu.GUI.Text
		GUI["d4"] = Instance.new("TextLabel", GUI["d0"]);
		GUI["d4"]["TextWrapped"] = true;
		GUI["d4"]["BorderSizePixel"] = 0;
		GUI["d4"]["TextSize"] = 45;
		GUI["d4"]["TextScaled"] = true;
		GUI["d4"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["d4"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		GUI["d4"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["d4"]["BackgroundTransparency"] = 2;
		GUI["d4"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		GUI["d4"]["Size"] = UDim2.new(0, 250, 0, 88);
		GUI["d4"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["d4"]["Text"] = [[DarkWave Hub]];
		GUI["d4"]["Name"] = [[TextLoader]];
		GUI["d4"]["Position"] = UDim2.new(0.50741, 0, 0.5, 0);
		
		GUI["d4"].Font = Enum.Font.GothamSemibold

		-- StarterGui.NewMenu.GUI.Line
		GUI["d5"] = Instance.new("Frame", GUI["d0"]);
		GUI["d5"]["BorderSizePixel"] = 0;
		GUI["d5"]["BackgroundColor3"] = Color3.fromRGB(200,200,200);
		GUI["d5"]["Size"] = UDim2.new(0, 200, 0, 1);
		GUI["d5"]["Position"] = UDim2.new(0.16296, 0, 0.5037, 0);
		GUI["d5"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["d5"]["Name"] = [[Line]];

		--LoaderSG
		task.wait(1.5)
		--Local

		local Main = GUI["d0"]
		local TextHub = GUI["d4"]
		local Line = GUI["d5"]
		local LoaderSG = GUI["1"]
		local DarkWaveSG = GUI["1"]
		local DMain = GUI["2"]
		local Container = GUI["10"]
		local Navigation = GUI["c3"] 



		local TextTime = 0.75
		local TextTime2 = 1
		local TextTimeTran = 1.25

		local LineTime = TextTime
		local LineTime2 = TextTime2
		local LineTimeTran = TextTimeTran


		local MainTime = 0.75
		local MainTimeMini = 0.5

		local MainSize = UDim2.new(0,250, 0,250)
		local MainMiniSize = UDim2.new(0,0, 0,0)

		local TextPosition1 = UDim2.new(0.504,0, 0.5,0)
		local LinePosition1 = UDim2.new(0.111,0, 0.504,0)


		local TextTransparency = 1
		local TextTransparency2 = 0
		local LineTransparency = TextTransparency
		local LineTransparency2 = TextTransparency2

		--Main Script
		Main.Visible = false
		TextHub.Visible = true
		Line.Visible = true

		Main.ClipsDescendants = true

		TextHub.Position = UDim2.new(1.3,0, 0.5,0)
		Line.Position = UDim2.new(1.1,0, 0.504,0)

		TextHub.Transparency = 1

		LoaderSG.Enabled = true

		if Main.Visible == false then

			Main.Visible = true
			task.wait(0.1)
			Main:TweenSize(MainSize, "Out", "Quad", MainTime, true)

		end

		task.wait(0.75)

		local TextTween1 = ts:Create(
			TextHub,
			TweenInfo.new(
				TextTime,
				Enum.EasingStyle.Quad,
				Enum.EasingDirection.Out,
				0,
				false,
				0
			),
			{
				Position = TextPosition1
			}
		)

		local LineTween1 = ts:Create(
			Line,
			TweenInfo.new(
				LineTime,
				Enum.EasingStyle.Quad,
				Enum.EasingDirection.Out,
				0,
				false,
				0
			),
			{
				Position = LinePosition1
			}
		)

		local TextTween3 = ts:Create(
			TextHub,
			TweenInfo.new(
				TextTimeTran,
				Enum.EasingStyle.Quad,
				Enum.EasingDirection.Out,
				0,
				false,
				0
			),
			{
				TextTransparency = TextTransparency2
			}
		)

		local LineTween3 = ts:Create(
			Line,
			TweenInfo.new(
				LineTimeTran,
				Enum.EasingStyle.Quad,
				Enum.EasingDirection.InOut,
				0,
				false,
				0
			),
			{
				Transparency = LineTransparency2
			}
		)

		local TextTween2 = ts:Create(
			TextHub,
			TweenInfo.new(
				TextTime2,
				Enum.EasingStyle.Quad,
				Enum.EasingDirection.InOut,
				0,
				false,
				0
			),
			{
				TextTransparency = TextTransparency
			}
		)

		local LineTween2 = ts:Create(
			Line,
			TweenInfo.new(
				LineTime2,
				Enum.EasingStyle.Quad,
				Enum.EasingDirection.InOut,
				0,
				false,
				0
			),
			{
				Transparency = LineTransparency
			}
		)

		TextTween1:Play()
		TextTween3:Play()
		task.wait(0.75)
		LineTween1:Play()
		LineTween3:Play()
		task.wait(1.5)
		TextTween2:Play()
		LineTween2:Play()
		task.wait(TextTime + 0.25)

		if players.LocalPlayer.PlayerGui[LoaderOptions.Name] then
			players.LocalPlayer.PlayerGui[LoaderOptions.Name]:Destroy()
			Main:TweenSize(MainMiniSize, "Out", "Quad", MainTimeMini, true)
			task.wait(MainTimeMini)
			Main.Visible = false
		else
			Main:TweenSize(MainMiniSize, "Out", "Quad", MainTimeMini, true)
			task.wait(MainTimeMini)
			Main.Visible = false
		end


		task.wait(0.5)
		------------------------------------------------------------------------------------------------


		local DMainTime = 1
		local NavTime = 1.75
		local ConTime = 1.75
		
		local DMainSize = DMain.Size
		local DMainMiniSize = UDim2.new(0,0, 0,0)

		local NavPosition1 = UDim2.new(0,3, 0,35)
		local NavPosition2 = UDim2.new(0,-250, 0,35)

		local ConPosition1 = UDim2.new(0,110, 0,35)
		local ConPosition2 = UDim2.new(1,0, 0,35)


		--Main Script

		Navigation.Visible = true
		DMain.Visible = false
		Container.Visible = true

		DMain.ClipsDescendants = true

		DarkWaveSG.Enabled = true

		Navigation.Position = NavPosition2
		Container.Position = ConPosition2

		DMain.Size = DMainMiniSize



		if DMain.Visible == false then
			DMain.Visible = true
			DMain:TweenSize(DMainSize, "Out", "Quad", DMainTime, true)
		end


		local NavTween = ts:Create(
			Navigation,
			TweenInfo.new(
				NavTime,
				Enum.EasingStyle.Quad,
				Enum.EasingDirection.InOut,
				0,
				false,
				0
			),
			{
				Position = NavPosition1
			}
		)

		local ConTween = ts:Create(
			Container,
			TweenInfo.new(
				ConTime,
				Enum.EasingStyle.Quad,
				Enum.EasingDirection.InOut,
				0,
				false,
				0
			),
			{
				Position = ConPosition1
			}
		)


		task.wait(0.75)
		NavTween:Play()
		task.wait(0.25)
		ConTween:Play()

	else
GUI["2"]["Visible"] = true
	end
	
	
	local dragging
	local dragInput
	local dragStart
	local startPos

	local function Lerp(a, b, m)
		return a + (b - a) * m
	end;

	local lastMousePos
	local lastGoalPos
	local DRAG_SPEED = (8); -- // The speed of the UI darg.
	local function Update(dt)
		if not (startPos) then return end;
		if not (dragging) and (lastGoalPos) then
			GUI["2"].Position = UDim2.new(startPos.X.Scale, Lerp(GUI["2"].Position.X.Offset, lastGoalPos.X.Offset, dt * DRAG_SPEED), startPos.Y.Scale, Lerp(GUI["2"].Position.Y.Offset, lastGoalPos.Y.Offset, dt * DRAG_SPEED))
			return 
		end;

		local delta = (lastMousePos - uis:GetMouseLocation())
		local xGoal = (startPos.X.Offset - delta.X);
		local yGoal = (startPos.Y.Offset - delta.Y);
		lastGoalPos = UDim2.new(startPos.X.Scale, xGoal, startPos.Y.Scale, yGoal)
		GUI["2"].Position = UDim2.new(startPos.X.Scale, Lerp(GUI["2"].Position.X.Offset, xGoal, dt * DRAG_SPEED), startPos.Y.Scale, Lerp(GUI["2"].Position.Y.Offset, yGoal, dt * DRAG_SPEED))
	end;

	GUI["4"].InputBegan:Connect(function(input)
		if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
			dragging = true
			dragStart = input.Position
			startPos = GUI["2"].Position
			lastMousePos = uis:GetMouseLocation()

			input.Changed:Connect(function()
				if input.UserInputState == Enum.UserInputState.End then
					dragging = false
				end
			end)
		end
	end)

	GUI["2"].InputChanged:Connect(function(input)
		if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
			dragInput = input
		end
	end)

	runService.Heartbeat:Connect(Update)

	

	--Minimize
	local function Minimize()
		local time = 0.4

		GUI["10"]["Visible"] = false
		GUI["c3"]["Visible"] = false
		GUI["b1"]["Visible"] = false
		GUI["b2"]["Visible"] = true

		GUI["2"]["ClipsDescendants"] = true
		TweenService:Create(GUI["2"], TweenInfo.new(time), {Size = UDim2.new(0,600, 0,35)}):Play()


	end



	--Close
	local function Close()
		GUI["1"]:Destroy()
	end

	--Close
	function GUI:Close()
		GUI["1"]:Destroy()
	end


	--Minimize
	function GUI:Minimize()
		local time = 0.4

		GUI["10"]["Visible"] = false
		GUI["c3"]["Visible"] = false
		GUI["b1"]["Visible"] = false
		GUI["b2"]["Visible"] = true

		GUI["2"]["ClipsDescendants"] = true
		TweenService:Create(GUI["2"], TweenInfo.new(time), {Size = UDim2.new(0,600, 0,35)}):Play()


	end

	--Open

	local function Open()
		local time = 0.4

		GUI["10"].Visible = true
		GUI["c3"].Visible = true
		GUI["b2"]["Visible"] = false
		GUI["b1"]["Visible"] = true

		TweenService:Create(GUI["2"], TweenInfo.new(time), {Size = UDim2.new(0,600, 0,375)}):Play()
		task.wait(time)
		GUI["2"]["ClipsDescendants"] = false

	end

	--GUI Logic (Minimize, Open, Close)
	GUI["b"].MouseButton1Click:Connect(Close)
	GUI["b1"].MouseButton1Click:Connect(Minimize)
	GUI["b2"].MouseButton1Click:Connect(Open)
	
	
	
	
	
	
	
	
	--Logic/Tabs
	function GUI:CreateTab(options)
		--Tabs
		
		
		local Tab = {
			Hover = false,
			Active = false
			}
		local Section = {}
		local Toggle = {}
		local Button = {}
		local Bind = {}
		local Textbox = {}
		local Slider = {}
		local Dropdown = {}
		local ColorPicker = {}
		local Notification = {}
		local Loader = {}
		local Label = {}
		local Warning = {}
		
		if GUI.CurrentTab == nil then
			GUI.CurrentTab = Tab
		end
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		

		--Render
		do	
			-- StarterGui.NewMenu.Main.Navigation.TestTab
			Tab["c8"] = Instance.new("Frame", GUI["c3"]);
			Tab["c8"]["BorderSizePixel"] = 0;
			Tab["c8"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
			Tab["c8"]["Selectable"] = true;
			Tab["c8"]["Size"] = UDim2.new(0, 95, 0, 25);
			Tab["c8"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Tab["c8"]["Name"] = options.Name;
			Tab["c8"]["BackgroundTransparency"] = 1;
			


			-- StarterGui.NewMenu.Main.Navigation.TestTab.NameTab
			Tab["c9"] = Instance.new("TextLabel", Tab["c8"]);
			Tab["c9"]["TextWrapped"] = true;
			Tab["c9"]["BorderSizePixel"] = 0;
			Tab["c9"]["TextSize"] = 14;
			Tab["c9"]["TextScaled"] = true;
			Tab["c9"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Tab["c9"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Tab["c9"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Tab["c9"]["BackgroundTransparency"] = 1;
			Tab["c9"]["Size"] = UDim2.new(0, 70, 0, 25);
			Tab["c9"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Tab["c9"]["Text"] = options.Name;
			Tab["c9"]["Name"] = [[NameTab]];
			Tab["c9"]["Position"] = UDim2.new(0.25, 0, 0, 0);


			Tab["c9"].Font = Enum.Font.GothamSemibold



			-- StarterGui.NewMenu.Main.Navigation.TestTab.ImageTab
			Tab["cb"] = Instance.new("ImageLabel", Tab["c8"]);
			Tab["cb"]["BorderSizePixel"] = 0;
			Tab["cb"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Tab["cb"]["Image"] = options.icon;
			Tab["cb"]["Size"] = UDim2.new(0, 23, 0, 23);
			Tab["cb"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Tab["cb"]["BackgroundTransparency"] = 1;
			Tab["cb"]["Name"] = [[ImageTab]];
			Tab["cb"]["Position"] = UDim2.new(0, 1, 0, 1);


			-- StarterGui.NewMenu.Main.Navigation.TestTab.UIStroke
			Tab["cd"] = Instance.new("UIStroke", Tab["c8"]);
			Tab["cd"]["Transparency"] = 1;
			Tab["cd"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
			Tab["cd"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterGui.NewMenu.Main.Navigation.TestTab.Button
			Tab["ce"] = Instance.new("TextButton", Tab["c8"]);
			Tab["ce"]["TextWrapped"] = true;
			Tab["ce"]["Active"] = false;
			Tab["ce"]["BorderSizePixel"] = 0;
			Tab["ce"]["TextColor3"] = Color3.fromRGB(151, 151, 151);
			Tab["ce"]["TextTransparency"] = 1;
			Tab["ce"]["TextSize"] = 14;
			Tab["ce"]["TextScaled"] = true;
			Tab["ce"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
			Tab["ce"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Tab["ce"]["Size"] = UDim2.new(0, 100, 0, 25);
			Tab["ce"]["BackgroundTransparency"] = 1;
			Tab["ce"]["Name"] = [[Button]];
			Tab["ce"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Tab["ce"]["Text"] = [[]];


			-- StarterGui.NewMenu.Main.Navigation.TestTab.UICorner
			Tab["cf"] = Instance.new("UICorner", Tab["c8"]);
			
			------------------
			
			-- StarterGui.NewMenu.Main.Container.TestTab
			Tab["13"] = Instance.new("ScrollingFrame", GUI["10"]);
			Tab["13"]["BorderSizePixel"] = 0;
			Tab["13"]["CanvasSize"] = UDim2.new(0, 0, 0, 1);
			Tab["13"]["CanvasPosition"] = Vector2.new(4, 0);
			Tab["13"]["TopImage"] = [[rbxassetid://7445543667]];
			Tab["13"]["MidImage"] = [[rbxassetid://7445543667]];
			Tab["13"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Tab["13"]["Name"] = options.Name;
			Tab["13"]["Selectable"] = false;
			Tab["13"]["BottomImage"] = [[rbxassetid://7445543667]];
			Tab["13"]["AutomaticCanvasSize"] = Enum.AutomaticSize.Y;
			Tab["13"]["Size"] = UDim2.new(0, 483, 0, 330);
			Tab["13"]["ScrollBarImageColor3"] = Color3.fromRGB(41, 41, 41);
			Tab["13"]["Position"] = UDim2.new(0, 0, 0, 3);
			Tab["13"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Tab["13"]["ScrollBarThickness"] = 4;
			Tab["13"]["BackgroundTransparency"] = 1;
			Tab["13"]["Visible"] = false;

			-- StarterGui.NewMenu.Main.Container.TestTab.UICorner
			Tab["14"] = Instance.new("UICorner", Tab["13"]);



			-- StarterGui.NewMenu.Main.Container.TestTab.UIListLayout
			Tab["15"] = Instance.new("UIListLayout", Tab["13"]);
			Tab["15"]["Padding"] = UDim.new(0, 5);
			Tab["15"]["SortOrder"] = Enum.SortOrder.LayoutOrder;


			-- StarterGui.NewMenu.Main.Container.TestTab.UIPadding
			Tab["16"] = Instance.new("UIPadding", Tab["13"]);
			Tab["16"]["PaddingTop"] = UDim.new(0, 1);
			Tab["16"]["PaddingLeft"] = UDim.new(0, 7);
			Tab["16"]["PaddingBottom"] = UDim.new(0, 9);
		end
		--Methods
		function Tab:Activate()
			if not Tab.Active then
				if GUI.CurrentTab ~= nil then
					GUI.CurrentTab:Deactivate()
				end
				Tab["c8"].BackgroundColor3 = Color3.new(0.137255, 0.137255, 0.137255)
				Tab["cd"].Color = Color3.new(0.137255, 0.137255, 0.137255)
				TweenService:Create(Tab["c8"], TweenInfo.new(0.4), {BackgroundTransparency = 0}):Play()
				TweenService:Create(Tab["cd"], TweenInfo.new(0.4), {Transparency = 0}):Play()
				Tab.Active = true
				Tab["13"].Visible = true

				GUI.CurrentTab = Tab
			end
		end
		function Tab:Deactivate()
			if Tab.Active then
				Tab.Active = false
				Tab.Hover = false
				Tab["13"].Visible = false
				
				Tab["c8"].BackgroundColor3 = Color3.new(0.137255, 0.137255, 0.137255)
				Tab["cd"].Color = Color3.new(0.137255, 0.137255, 0.137255)
				TweenService:Create(Tab["c8"], TweenInfo.new(0.4), {BackgroundTransparency = 1}):Play()
				TweenService:Create(Tab["cd"], TweenInfo.new(0.4), {Transparency = 1}):Play()
			end
		end
		

--Section
			function Tab:CreateSection(options)
				


				--Render
				
					-- StarterSection.NewMenu.Main.Container.TestTab.Section
					Section["17"] = Instance.new("Frame", Tab["13"]);
					Section["17"]["BorderSizePixel"] = 0;
					Section["17"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
					Section["17"]["Size"] = UDim2.new(0, 465, 0, 20);
					Section["17"]["Position"] = UDim2.new(0, 0, 0.0152, 0);
					Section["17"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
					Section["17"]["Name"] = options.Text;
					Section["17"]["BackgroundTransparency"] = 1;


					-- StarterSection.NewMenu.Main.Container.TestTab.Section.UICorner
					Section["18"] = Instance.new("UICorner", Section["17"]);



					-- StarterSection.NewMenu.Main.Container.TestTab.Section.SectionName
					Section["19"] = Instance.new("TextLabel", Section["17"]);
					Section["19"]["TextWrapped"] = true;
					Section["19"]["BorderSizePixel"] = 0;
					Section["19"]["TextSize"] = 14;
					Section["19"]["TextXAlignment"] = Enum.TextXAlignment.Left;
					Section["19"]["TextScaled"] = true;
					Section["19"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
					Section["19"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
					Section["19"]["TextColor3"] = Color3.fromRGB(76, 76, 76);
					Section["19"]["BackgroundTransparency"] = 1;
					Section["19"]["Size"] = UDim2.new(0, 465, 0, 17);
					Section["19"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
					Section["19"]["Text"] = options.Text;
					Section["19"]["Name"] = [[SectionName]];
					Section["19"]["Position"] = UDim2.new(0, 0, 0, 5);


					-- StarterSection.NewMenu.Main.Container.TestTab.Section.SectionName.LocalScript
					Section["1a"] = Instance.new("LocalScript", Section["19"]);
				
				return Section
			end


--Toggle

	function Tab:CreateToggle(options)
		--Logic
			local Callback = options.Callback or function() end
			
			--Render
			
			-- StarterToggle.NewMenu.Main.Container.TestToggle.Toggle
			Toggle["1b"] = Instance.new("Frame", Tab["13"]);
			Toggle["1b"]["BorderSizePixel"] = 0;
			Toggle["1b"]["BackgroundColor3"] = Color3.fromRGB(31, 31, 31);
			Toggle["1b"]["Size"] = UDim2.new(0, 465, 0, 35);
			Toggle["1b"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Toggle["1b"]["Name"] = options.Name;
			Toggle["1b"]["BackgroundTransparency"] = 1;


			-- StarterToggle.NewMenu.Main.Container.TestToggle.Toggle.UIStroke
			Toggle["1c"] = Instance.new("UIStroke", Toggle["1b"]);
			Toggle["1c"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterToggle.NewMenu.Main.Container.TestToggle.Toggle.UICorner
			Toggle["1d"] = Instance.new("UICorner", Toggle["1b"]);



			-- StarterToggle.NewMenu.Main.Container.TestToggle.Toggle.ToggleName
			Toggle["1e"] = Instance.new("TextLabel", Toggle["1b"]);
			Toggle["1e"]["TextWrapped"] = true;
			Toggle["1e"]["BorderSizePixel"] = 0;
			Toggle["1e"]["TextSize"] = 14;
			Toggle["1e"]["TextXAlignment"] = Enum.TextXAlignment.Left;
			Toggle["1e"]["TextScaled"] = true;
			Toggle["1e"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Toggle["1e"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Toggle["1e"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Toggle["1e"]["BackgroundTransparency"] = 1;
			Toggle["1e"]["Size"] = UDim2.new(0, 420, 0, 25);
			Toggle["1e"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Toggle["1e"]["Text"] = options.Name;
			Toggle["1e"]["Name"] = options.Name;
			Toggle["1e"]["Position"] = UDim2.new(0, 3, 0.15, 0);


			-- StarterToggle.NewMenu.Main.Container.TestToggle.Toggle.ToggleName.LocalScript
			Toggle["1e"].Font = Enum.Font.GothamSemibold



			-- StarterToggle.NewMenu.Main.Container.TestToggle.Toggle.CheckBox
			Toggle["20"] = Instance.new("TextButton", Toggle["1b"]);
			Toggle["20"]["Active"] = false;
			Toggle["20"]["BorderSizePixel"] = 0;
			Toggle["20"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Toggle["20"]["Size"] = UDim2.new(0, 30, 0, 30);
			Toggle["20"]["BackgroundTransparency"] = 1;
			Toggle["20"]["Name"] = [[CheckBox]];
			Toggle["20"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Toggle["20"]["Text"] = [[]];
			Toggle["20"]["Position"] = UDim2.new(0, 430, 0, 2);


			-- StarterToggle.NewMenu.Main.Container.TestToggle.Toggle.CheckBox.UIStroke
			Toggle["21"] = Instance.new("UIStroke", Toggle["20"]);
			Toggle["21"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
			Toggle["21"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterToggle.NewMenu.Main.Container.TestToggle.Toggle.CheckBox.UICorner
			Toggle["22"] = Instance.new("UICorner", Toggle["20"]);



			-- StarterToggle.NewMenu.Main.Container.TestToggle.Toggle.CheckBox.CheckMark
			Toggle["23"] = Instance.new("ImageLabel", Toggle["20"]);
			Toggle["23"]["BorderSizePixel"] = 0;
			Toggle["23"]["SliceScale"] = 0;
			Toggle["23"]["BackgroundColor3"] = Color3.fromRGB(10, 100, 196);
			Toggle["23"]["ImageTransparency"] = 1;
			Toggle["23"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
			Toggle["23"]["Image"] = [[rbxassetid://10709790644]];
			Toggle["23"]["TileSize"] = UDim2.new(0, 10, 0, 10);
			Toggle["23"]["Size"] = UDim2.new(0, 30, 0, 30);
			Toggle["23"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Toggle["23"]["BackgroundTransparency"] = 1;
			Toggle["23"]["Name"] = [[CheckMark]];
			Toggle["23"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);


			-- StarterToggle.NewMenu.Main.Container.TestToggle.Toggle.CheckBox.CheckMark.UICorner
			Toggle["24"] = Instance.new("UICorner", Toggle["23"]);



			-- StarterToggle.NewMenu.Main.Container.TestToggle.Toggle.CheckBox.Button
			Toggle["25"] = Instance.new("TextButton", Toggle["20"]);
			Toggle["25"]["Active"] = false;
			Toggle["25"]["BorderSizePixel"] = 0;
			Toggle["25"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Toggle["25"]["Size"] = UDim2.new(0, 457, 0, 30);
			Toggle["25"]["BackgroundTransparency"] = 1;
			Toggle["25"]["Name"] = [[Button]];
			Toggle["25"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Toggle["25"]["Text"] = [[]];
			Toggle["25"]["Position"] = UDim2.new(-14.23333, 0, 0, 0);


			-- StarterToggle.NewMenu.Main.Container.TestToggle.Toggle.CheckBox.Button.UICorner
			Toggle["26"] = Instance.new("UICorner", Toggle["25"]);



				-- StarterTab.NewMenu.Main.Container.TestTab.Toggle.CheckBox.Button.LocalScript
			local EnabledFrM = false
			
			local time = 0.2

			if options.Default == false then
				options.Value = false
				Toggle["23"].ImageTransparency = 1
				Toggle["23"].BackgroundTransparency = 1
			elseif options.Default == true then
				options.Value = true
				Toggle["23"].ImageTransparency = 0
				Toggle["23"].BackgroundTransparency = 0
			end
			Toggle["25"].MouseButton1Click:Connect(function()
				if EnabledFrM == false and Toggle["23"].Transparency == 1 then
					EnabledFrM = true
					local tween1 = TweenService:Create(Toggle["23"], TweenInfo.new(time), {ImageTransparency = 0, BackgroundTransparency = 0})
					tween1:Play()
					
					options.Value = EnabledFrM
					Callback(options.Value)
				elseif EnabledFrM == true and Toggle["23"].Transparency == 0 then
					local tween2 = TweenService:Create(Toggle["23"], TweenInfo.new(time), {ImageTransparency = 1, BackgroundTransparency = 1})
					tween2:Play()
					task.wait(time)
					EnabledFrM = false
					
					options.Value = EnabledFrM
					Callback(options.Value)
				elseif EnabledFrM == false and Toggle["23"].Transparency == 0 then
					EnabledFrM = true
					local tween1 = TweenService:Create(Toggle["23"], TweenInfo.new(time), {ImageTransparency = 0, BackgroundTransparency = 0})
					tween1:Play()
					
					options.Value = EnabledFrM
					Callback(options.Value)
				elseif EnabledFrM == true and Toggle["23"].Transparency == 1 then
					EnabledFrM = false
					local tween2 = TweenService:Create(Toggle["23"], TweenInfo.new(time), {ImageTransparency = 1, BackgroundTransparency = 1})
					tween2:Play()
					task.wait(time)
					
					options.Value = EnabledFrM
					Callback(options.Value)
				end
			end)
			


				-- StarterTab.NewMenu.Main.Container.TestTab.Toggle.LocalScript

			Toggle["1b"].BackgroundColor3 = Color3.fromRGB(30,30,30)
			Toggle["1b"].BackgroundTransparency = 1

			Toggle["1b"].MouseEnter:Connect(function()
				TweenService:Create(Toggle["1b"], TweenInfo.new(0.4), {BackgroundTransparency = 0}):Play()
			end)


			Toggle["1b"].MouseLeave:Connect(function()
				TweenService:Create(Toggle["1b"], TweenInfo.new(0.4), {BackgroundTransparency = 1}):Play()
			end)
			
			function Toggle:Set(Value)
				if Value == false then
					TweenService:Create(Toggle["23"], TweenInfo.new(time), {ImageTransparency = 1, BackgroundTransparency = 1}):Play()
				elseif Value == true then
					TweenService:Create(Toggle["23"], TweenInfo.new(time), {ImageTransparency = 0, BackgroundTransparency = 0}):Play()
				else
					Value = false
					TweenService:Create(Toggle["23"], TweenInfo.new(time), {ImageTransparency = 1, BackgroundTransparency = 1}):Play()
				end
				

			end  

			return Toggle
	end

  



	
	--Button
	
	function Tab:CreateButton(options)
			local Callback = options.Callback or function() end
			--Render
			-- StarterButton.NewMenu.Main.Container.TestTab.Button
			Button["57"] = Instance.new("Frame", Tab["13"]);
			Button["57"]["BorderSizePixel"] = 0;
			Button["57"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Button["57"]["Size"] = UDim2.new(0, 465, 0, 35);
			Button["57"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Button["57"]["Name"] = options.Name;
			Button["57"]["BackgroundTransparency"] = 1;


			-- StarterButton.NewMenu.Main.Container.TestTab.Button.UIStroke
			Button["58"] = Instance.new("UIStroke", Button["57"]);
			Button["58"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
			Button["58"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterButton.NewMenu.Main.Container.TestTab.Button.UICorner
			Button["59"] = Instance.new("UICorner", Button["57"]);



			-- StarterButton.NewMenu.Main.Container.TestTab.Button.ButtonName
			Button["5a"] = Instance.new("TextLabel", Button["57"]);
			Button["5a"]["TextWrapped"] = true;
			Button["5a"]["BorderSizePixel"] = 0;
			Button["5a"]["TextSize"] = 14;
			Button["5a"]["TextXAlignment"] = Enum.TextXAlignment.Left;
			Button["5a"]["TextScaled"] = true;
			Button["5a"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Button["5a"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Button["5a"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Button["5a"]["BackgroundTransparency"] = 1;
			Button["5a"]["Size"] = UDim2.new(0, 420, 0, 25);
			Button["5a"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Button["5a"]["Text"] = options.Name;
			Button["5a"]["Name"] = [[ButtonName]];
			Button["5a"]["Position"] = UDim2.new(0, 3, 0.15, 0);


			-- StarterButton.NewMenu.Main.Container.TestTab.Button.ButtonName.LocalScript
			Button["5a"].Font = Enum.Font.GothamSemibold





			-- StarterButton.NewMenu.Main.Container.TestTab.Button.Image
			Button["5c"] = Instance.new("ImageLabel", Button["57"]);
			Button["5c"]["BorderSizePixel"] = 0;
			Button["5c"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Button["5c"]["Image"] = [[rbxassetid://10734898355]];
			Button["5c"]["Size"] = UDim2.new(0, 35, 0, 35);
			Button["5c"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Button["5c"]["BackgroundTransparency"] = 1;
			Button["5c"]["Name"] = [[Image]];
			Button["5c"]["Position"] = UDim2.new(0, 424, 0, 0);


			-- StarterButton.NewMenu.Main.Container.TestTab.Button.Button
			Button["5d"] = Instance.new("TextButton", Button["57"]);
			Button["5d"]["Active"] = false;
			Button["5d"]["BorderSizePixel"] = 0;
			Button["5d"]["TextTransparency"] = 1;
			Button["5d"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Button["5d"]["Selectable"] = false;
			Button["5d"]["Size"] = UDim2.new(0, 465, 0, 35);
			Button["5d"]["BackgroundTransparency"] = 1;
			Button["5d"]["Name"] = [[Button]];
			Button["5d"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Button["5d"]["Text"] = [[]];


			-- StarterButton.NewMenu.Main.Container.TestTab.Button.Button.UICorner
			Button["5e"] = Instance.new("UICorner", Button["5d"]);



			-- StarterGui.NewMenu.Main.Container.TestTab.Button.LocalScript
			Button["57"].BackgroundColor3 = Color3.fromRGB(30,30,30)
			Button["57"].BackgroundTransparency = 1

			Button["57"].MouseEnter:Connect(function()
				TweenService:Create(Button["57"], TweenInfo.new(0.4), {BackgroundTransparency = 0}):Play()
			end)


			Button["57"].MouseLeave:Connect(function()
				TweenService:Create(Button["57"], TweenInfo.new(0.4), {BackgroundTransparency = 1}):Play()
			end)
			
			Button["5d"].MouseButton1Click:Connect(function()
				Callback()
			end)
			
			return Button
	end
	
	--Bind
	
	function Tab:CreateBind(options)
			local Callback = options.Callback or function() end
			--Render
			-- StarterBind.NewMenu.Main.Container.TestTab.Bind
			
Bind["41"] = Instance.new("Frame", Tab["13"]);
			Bind["41"]["BorderSizePixel"] = 0;
			Bind["41"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Bind["41"]["Size"] = UDim2.new(0, 465, 0, 35);
			Bind["41"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Bind["41"]["Name"] = options.Name;
			Bind["41"]["BackgroundTransparency"] = 1;


			-- StarterBind.NewMenu.Main.Container.TestTab.Bind.UIStroke
			Bind["42"] = Instance.new("UIStroke", Bind["41"]);
			Bind["42"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterBind.NewMenu.Main.Container.TestTab.Bind.UICorner
			Bind["43"] = Instance.new("UICorner", Bind["41"]);



			-- StarterBind.NewMenu.Main.Container.TestTab.Bind.BindName
			Bind["44"] = Instance.new("TextLabel", Bind["41"]);
			Bind["44"]["TextWrapped"] = true;
			Bind["44"]["BorderSizePixel"] = 0;
			Bind["44"]["TextSize"] = 14;
			Bind["44"]["TextXAlignment"] = Enum.TextXAlignment.Left;
			Bind["44"]["TextScaled"] = true;
			Bind["44"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Bind["44"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Bind["44"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Bind["44"]["BackgroundTransparency"] = 1;
			Bind["44"]["Size"] = UDim2.new(0, 371, 0, 25);
			Bind["44"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Bind["44"]["Text"] = options.Name;
			Bind["44"]["Name"] = [[BindName]];
			Bind["44"]["Position"] = UDim2.new(0, 3, 0.15, 0);


			-- StarterBind.NewMenu.Main.Container.TestTab.Bind.BindName.LocalScript
			Bind["45"] = Instance.new("LocalScript", Bind["44"]);



			-- StarterBind.NewMenu.Main.Container.TestTab.Bind.LocalScript
			Bind["41"].BackgroundColor3 = Color3.fromRGB(30,30,30)
			Bind["41"].BackgroundTransparency = 1

			Bind["41"].MouseEnter:Connect(function()
				TweenService:Create(Bind["41"], TweenInfo.new(0.4), {BackgroundTransparency = 0}):Play()
			end)


			Bind["41"].MouseLeave:Connect(function()
				TweenService:Create(Bind["41"], TweenInfo.new(0.4), {BackgroundTransparency = 1}):Play()
			end)



			-- StarterBind.NewMenu.Main.Container.TestTab.Bind.KeyBind
			Bind["47"] = Instance.new("TextLabel", Bind["41"]);
			Bind["47"]["TextWrapped"] = true;
			Bind["47"]["BorderSizePixel"] = 0;
			Bind["47"]["TextScaled"] = true;
			Bind["47"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Bind["47"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Bind["47"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Bind["47"]["BackgroundTransparency"] = 1;
			Bind["47"]["Size"] = UDim2.new(0, 30, 0, 30);
			Bind["47"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Bind["47"]["Text"] = options.Default;
			Bind["47"]["Name"] = [[KeyBind]];
			Bind["47"]["Position"] = UDim2.new(0, 430, 0, 2);


			-- StarterBind.NewMenu.Main.Container.TestTab.Bind.KeyBind.UIStroke
			Bind["48"] = Instance.new("UIStroke", Bind["47"]);
			Bind["48"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
			Bind["48"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterBind.NewMenu.Main.Container.TestTab.Bind.KeyBind.UICorner
			Bind["49"] = Instance.new("UICorner", Bind["47"]);



			-- StarterBind.NewMenu.Main.Container.TestTab.Bind.KeyBind.LocalScript
			Bind["4a"] = Instance.new("LocalScript", Bind["47"]);



			-- StarterBind.NewMenu.Main.Container.TestTab.Bind.Button
			Bind["4b"] = Instance.new("TextButton", Bind["41"]);
			Bind["4b"]["Active"] = false;
			Bind["4b"]["BorderSizePixel"] = 0;
			Bind["4b"]["TextTransparency"] = 1;
			Bind["4b"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Bind["4b"]["Selectable"] = false;
			Bind["4b"]["Size"] = UDim2.new(0, 465, 0, 35);
			Bind["4b"]["BackgroundTransparency"] = 1;
			Bind["4b"]["Name"] = [[Button]];
			Bind["4b"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Bind["4b"]["Text"] = [[]];


			-- StarterBind.NewMenu.Main.Container.TestTab.Bind.Button.LocalScript
			local BindLock = false
			Bind["4b"].MouseButton1Click:Connect(function()
				Bind["47"].Text = "..."
				BindLock = true
				uis.InputBegan:Connect(function(input)
					if BindLock == true then
						if input.UserInputType == Enum.UserInputType.Keyboard then
							Bind["47"].Text = uis:GetStringForKeyCode(input.KeyCode) 
							BindLock = false
							Callback(uis:GetStringForKeyCode(input.KeyCode))
						end
					end
				end)
			end)
			return Bind
	end

--Textbox
	function Tab:CreateTextbox(options)
			local Callback = options.Callback or function() end
			-- StarterTextbox.NewMenu.Main.Container.TestTab.Textbox
			Textbox["4d"] = Instance.new("Frame", Tab["13"]);
			Textbox["4d"]["BorderSizePixel"] = 0;
			Textbox["4d"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Textbox["4d"]["Size"] = UDim2.new(0, 465, 0, 35);
			Textbox["4d"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Textbox["4d"]["Name"] = options.Name;
			Textbox["4d"]["BackgroundTransparency"] = 1;


			-- StarterTextbox.NewMenu.Main.Container.TestTab.Textbox.UIStroke
			Textbox["4e"] = Instance.new("UIStroke", Textbox["4d"]);
			Textbox["4e"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterTextbox.NewMenu.Main.Container.TestTab.Textbox.UICorner
			Textbox["4f"] = Instance.new("UICorner", Textbox["4d"]);



			-- StarterTextbox.NewMenu.Main.Container.TestTab.Textbox.TextboxName
			Textbox["50"] = Instance.new("TextLabel", Textbox["4d"]);
			Textbox["50"]["TextWrapped"] = true;
			Textbox["50"]["BorderSizePixel"] = 0;
			Textbox["50"]["TextSize"] = 14;
			Textbox["50"]["TextXAlignment"] = Enum.TextXAlignment.Left;
			Textbox["50"]["TextScaled"] = true;
			Textbox["50"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Textbox["50"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Textbox["50"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Textbox["50"]["BackgroundTransparency"] = 1;
			Textbox["50"]["Size"] = UDim2.new(0, 371, 0, 25);
			Textbox["50"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Textbox["50"]["Text"] = options.Name;
			Textbox["50"]["Name"] = [[TextboxName]];
			Textbox["50"]["Position"] = UDim2.new(0, 3, 0.15, 0);


			-- StarterTextbox.NewMenu.Main.Container.TestTab.Textbox.TextboxName.LocalScript
			Textbox["51"] = Instance.new("LocalScript", Textbox["50"]);



			-- StarterTextbox.NewMenu.Main.Container.TestTab.Textbox.Textbox
			Textbox["52"] = Instance.new("TextBox", Textbox["4d"]);
			Textbox["52"]["Active"] = false;
			Textbox["52"]["Name"] = [[Textbox]];
			Textbox["52"]["BorderSizePixel"] = 0;
			Textbox["52"]["TextWrapped"] = true;
			Textbox["52"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Textbox["52"]["TextScaled"] = true;
			Textbox["52"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Textbox["52"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Textbox["52"]["Selectable"] = false;
			Textbox["52"]["Size"] = UDim2.new(0, 75, 0, 30);
			Textbox["52"]["Position"] = UDim2.new(0, 385, 0, 2);
			Textbox["52"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Textbox["52"]["Text"] = options.Default;
			Textbox["52"]["BackgroundTransparency"] = 1;


			-- StarterTextbox.NewMenu.Main.Container.TestTab.Textbox.Textbox.UIStroke
			Textbox["53"] = Instance.new("UIStroke", Textbox["52"]);
			Textbox["53"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
			Textbox["53"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterTextbox.NewMenu.Main.Container.TestTab.Textbox.Textbox.UICorner
			Textbox["54"] = Instance.new("UICorner", Textbox["52"]);



			-- StarterTextbox.NewMenu.Main.Container.TestTab.Textbox.Textbox.LocalScript
			Textbox["4d"].BackgroundColor3 = Color3.fromRGB(30,30,30)
			Textbox["4d"].BackgroundTransparency = 1

			Textbox["4d"].MouseEnter:Connect(function()
				TweenService:Create(Textbox["4d"], TweenInfo.new(0.4), {BackgroundTransparency = 0}):Play()
			end)


			Textbox["4d"].MouseLeave:Connect(function()
				TweenService:Create(Textbox["4d"], TweenInfo.new(0.4), {BackgroundTransparency = 1}):Play()
			end)



			-- StarterTextbox.NewMenu.Main.Container.TestTab.Textbox.LocalScript
			if options.OnlyNumbers == true then
				
				local function stripNonNumbers()
					Textbox["52"].Text = Textbox["52"].Text:gsub("%D","")
				end
				Textbox["52"]:GetPropertyChangedSignal("Text"):Connect(stripNonNumbers)
				Textbox["52"]:GetPropertyChangedSignal("Text"):Connect(stripNonNumbers) 
				Textbox["52"].Text:gsub("%D","") 
				
				local lastFov = 100

				local function setFov()
					local newFov = tonumber(Textbox["52"].Text)
					if newFov then
						lastFov = newFov
					else
						Textbox["52"].Text = lastFov
					end
				end
				Textbox["52"].FocusLost:Connect(setFov)
			end
			
			uis.InputBegan:Connect(function(input)
				if input.UserInputType == Enum.KeyCode.Return or  Enum.KeyCode.KeypadEnter then
                    Callback(Textbox["52"].Text)
				end
			end)

return Textbox
	end

--Slider
function Tab:CreateSlider(options)
	local Callback = options.Callback or function() end
	
	--Render
			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider
			Slider["29"] = Instance.new("Frame", Tab["13"]);
			Slider["29"]["BorderSizePixel"] = 0;
			Slider["29"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Slider["29"]["Size"] = UDim2.new(0, 465, 0, 50);
			Slider["29"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Slider["29"]["Name"] = options.Name;
			Slider["29"]["BackgroundTransparency"] = 1;


			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.UIStroke
			Slider["2a"] = Instance.new("UIStroke", Slider["29"]);
			Slider["2a"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.UICorner
			Slider["2b"] = Instance.new("UICorner", Slider["29"]);



			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderName
			Slider["2c"] = Instance.new("TextLabel", Slider["29"]);
			Slider["2c"]["TextWrapped"] = true;
			Slider["2c"]["BorderSizePixel"] = 0;
			Slider["2c"]["TextSize"] = 14;
			Slider["2c"]["TextXAlignment"] = Enum.TextXAlignment.Left;
			Slider["2c"]["TextScaled"] = true;
			Slider["2c"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Slider["2c"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Slider["2c"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Slider["2c"]["BackgroundTransparency"] = 1;
			Slider["2c"]["Size"] = UDim2.new(0, 456, 0, 15);
			Slider["2c"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Slider["2c"]["Text"] = options.Name;
			Slider["2c"]["Name"] = [[SliderName]];
			Slider["2c"]["Position"] = UDim2.new(0.00215, 3, 0.07, 0);


			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderName.LocalScript
			Slider["2c"].Font = Enum.Font.GothamSemibold



			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame
			Slider["2e"] = Instance.new("Frame", Slider["29"]);
			Slider["2e"]["BorderSizePixel"] = 0;
			Slider["2e"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Slider["2e"]["Size"] = UDim2.new(0, 455, 0, 20);
			Slider["2e"]["Position"] = UDim2.new(0, 3, 0, 25);
			Slider["2e"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Slider["2e"]["Name"] = [[SliderFrame]];
			Slider["2e"]["BackgroundTransparency"] = 1;
			Slider["2e"]["ClipsDescendants"] = true;


			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.UICorner
			Slider["2f"] = Instance.new("UICorner", Slider["2e"]);



			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.UIStroke
			Slider["30"] = Instance.new("UIStroke", Slider["2e"]);
			Slider["30"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide
			Slider["31"] = Instance.new("Frame", Slider["2e"]);
			Slider["31"]["BorderSizePixel"] = 0;
			Slider["31"]["BackgroundColor3"] = Color3.fromRGB(31, 31, 31);
			Slider["31"]["Size"] = UDim2.new(0, 100, 0, 20);
			Slider["31"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Slider["31"]["Name"] = [[Slide]];


			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.UICorner
			Slider["32"] = Instance.new("UICorner", Slider["31"]);



			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.UIStroke
			Slider["33"] = Instance.new("UIStroke", Slider["31"]);
			Slider["33"]["Color"] = Color3.fromRGB(36, 36, 36);

			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.OutputValue
			Slider["35"] = Instance.new("IntValue", Slider["31"]);
			Slider["35"]["Name"] = [[OutputValue]];


			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.Trigger
			Slider["36"] = Instance.new("TextButton", Slider["31"]);
			Slider["36"]["BorderSizePixel"] = 0;
			Slider["36"]["BackgroundColor3"] = Color3.fromRGB(31, 31, 31);
			Slider["36"]["Selectable"] = false;
			Slider["36"]["Size"] = UDim2.new(0, 456, 0, 20);
			Slider["36"]["BackgroundTransparency"] = 1;
			Slider["36"]["Name"] = [[Trigger]];
			Slider["36"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Slider["36"]["Text"] = [[]];
			Slider["36"]["Position"] = UDim2.new(0, 0, 0, 0);


			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.Trigger.UICorner
			Slider["37"] = Instance.new("UICorner", Slider["36"]);



			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.Trigger.UIStroke
			Slider["38"] = Instance.new("UIStroke", Slider["36"]);
			Slider["38"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.Main
			Slider["39"] = Instance.new("Frame", Slider["31"]);
			Slider["39"]["BorderSizePixel"] = 0;
			Slider["39"]["BackgroundColor3"] = Color3.fromRGB(31, 31, 31);
			Slider["39"]["Size"] = UDim2.new(0, 80, 0, 20);
			Slider["39"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Slider["39"]["Name"] = [[Main]];
			Slider["39"]["BackgroundTransparency"] = 1;


			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.Main.ValueText
			Slider["3a"] = Instance.new("TextLabel", Slider["39"]);
			Slider["3a"]["TextWrapped"] = true;
			Slider["3a"]["BorderSizePixel"] = 0;
			Slider["3a"]["TextSize"] = 14;
			Slider["3a"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Slider["3a"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Slider["3a"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Slider["3a"]["BackgroundTransparency"] = 1;
			Slider["3a"]["Size"] = UDim2.new(0, 30, 0, 20);
			Slider["3a"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Slider["3a"]["Text"] = options.Default;
			Slider["3a"]["Name"] = [[ValueText]];


			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.Main.ValueText.UICorner
			Slider["3b"] = Instance.new("UICorner", Slider["3a"]);



			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.Main.ValueText.LocalScript
			Slider["3a"].Font = Enum.Font.GothamSemibold



			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.Main.Text
			Slider["3d"] = Instance.new("TextLabel", Slider["39"]);
			Slider["3d"]["TextWrapped"] = true;
			Slider["3d"]["BorderSizePixel"] = 0;
			Slider["3d"]["TextSize"] = 14;
			Slider["3d"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Slider["3d"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Slider["3d"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Slider["3d"]["BackgroundTransparency"] = 1;
			Slider["3d"]["Size"] = UDim2.new(0, 50, 0, 20);
			Slider["3d"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Slider["3d"]["Text"] = options.ValueName;
			Slider["3d"]["Name"] = [[Text]];
			Slider["3d"]["Position"] = UDim2.new(0.3, 0, 0, 0);


			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.Main.Text.UICorner
			Slider["3e"] = Instance.new("UICorner", Slider["3d"]);



			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.Main.Text.LocalScript
			Slider["3d"].Font = Enum.Font.GothamSemibold



			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.LocalScript
			
			
			Slider["29"].BackgroundColor3 = Color3.fromRGB(30,30,30)
			Slider["29"].BackgroundTransparency = 1

			Slider["29"].MouseEnter:Connect(function()
				TweenService:Create(Slider["29"], TweenInfo.new(0.4), {BackgroundTransparency = 0}):Play()
			end)


			Slider["29"].MouseLeave:Connect(function()
				TweenService:Create(Slider["29"], TweenInfo.new(0.4), {BackgroundTransparency = 1}):Play()
			end)

			
			
			-- StarterSlider.NewMenu.Main.Container.TestTab.Slider.SliderFrame.Slide.LocalScript


			local Mouse = game.Players.LocalPlayer:GetMouse()

			local TweenStyle = TweenInfo.new(0.25,Enum.EasingStyle.Exponential)
			Slider["35"].Value = options.Default
			Slider["31"].Size = UDim2.fromScale(0, Slider["35"].Value)
			Slider["3a"].Text = tostring(math.round(Slider["35"].Value))

			local function UpdateSlider()
				local output = math.clamp(((Vector2.new(Mouse.X,Mouse.Y)-Slider["2c"].AbsolutePosition)/Slider["2c"].AbsoluteSize).X,0,1)

				local outputClamped = options.Default + (output *(options.Maximum-options.Default))

				if Slider["35"].Value ~= outputClamped then
					TweenService:Create(Slider["31"],TweenStyle,{Size = UDim2.fromScale(output,1)}):Play()
				end

				Slider["35"].Value = options.Default + (output*(options.Maximum-options.Default))
				Slider["3a"].Text = tostring(math.round(outputClamped))
				
			end

			Slider["31"]:GetPropertyChangedSignal("Size"):Connect(function()
				Slider["3a"].Text = tostring(math.round(Slider["35"].Value))
				
			end)

			local sliderActive = false
			

			local function ActivateSlider()
				sliderActive = true
				while sliderActive do
					UpdateSlider()
					task.wait()
				end
				Callback(Slider["35"].Value)
			end

			Slider["36"].MouseButton1Down:Connect(ActivateSlider)

			uis.InputEnded:Connect(function(input)
				if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
					sliderActive = false
				end
			end)
			
			
			function Slider:Set(Value)
			if Value > options.Maximum then
			   Value = options.Maximum
				Slider["35"].Value = Value
				Slider["3a"].Text = tostring(Value)
				Slider["31"].Size = UDim2.new(0, Value, 0 , 20)
			elseif Value < options.Minimum then
				Value = options.Minimum
				Slider["35"].Value = Value
				Slider["3a"].Text = tostring(Value)
				Slider["31"].Size = UDim2.new(0, Value, 0 , 20)
			else
					Slider["35"].Value = Value
					Slider["3a"].Text = tostring(Value)
					Slider["31"].Size = UDim2.new(0, Value, 0 , 20)
			end
			
			end
			
			return Slider

end

--Dropdown
function Tab:CreateDropdown(options)
	
			local Callback = options.Callback or function() end
			
			
			local open = false
			local time = 0.3
			local Ysize = 115
	--Render
			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown
			Dropdown["60"] = Instance.new("Frame", Tab["13"]);
			Dropdown["60"]["BorderSizePixel"] = 0;
			Dropdown["60"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Dropdown["60"]["Size"] = UDim2.new(0, 465, 0, 35);
			Dropdown["60"]["Position"] = UDim2.new(0, 0, 0.12158, 0);
			Dropdown["60"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Dropdown["60"]["Name"] = options.Name;
			Dropdown["60"]["BackgroundTransparency"] = 1;


			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.UIStroke
			Dropdown["61"] = Instance.new("UIStroke", Dropdown["60"]);
			Dropdown["61"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
			Dropdown["61"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.UICorner
			Dropdown["62"] = Instance.new("UICorner", Dropdown["60"]);



			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.TopDropdown
			Dropdown["63"] = Instance.new("Frame", Dropdown["60"]);
			Dropdown["63"]["BorderSizePixel"] = 0;
			Dropdown["63"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
			Dropdown["63"]["Size"] = UDim2.new(0, 465, 0, 35);
			Dropdown["63"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Dropdown["63"]["Name"] = [[TopDropdown]];
			Dropdown["63"]["BackgroundTransparency"] = 1;


			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.TopDropdown.UIStroke
			Dropdown["64"] = Instance.new("UIStroke", Dropdown["63"]);
			Dropdown["64"]["Color"] = Color3.fromRGB(36, 36, 36);


			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.TopDropdown.UICorner
			Dropdown["65"] = Instance.new("UICorner", Dropdown["63"]);



			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.TopDropdown.DropdownName
			Dropdown["66"] = Instance.new("TextLabel", Dropdown["63"]);
			Dropdown["66"]["TextWrapped"] = true;
			Dropdown["66"]["BorderSizePixel"] = 0;
			Dropdown["66"]["TextSize"] = 14;
			Dropdown["66"]["TextXAlignment"] = Enum.TextXAlignment.Left;
			Dropdown["66"]["TextScaled"] = true;
			Dropdown["66"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Dropdown["66"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Dropdown["66"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Dropdown["66"]["BackgroundTransparency"] = 1;
			Dropdown["66"]["Size"] = UDim2.new(0, 370, 0, 25);
			Dropdown["66"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Dropdown["66"]["Text"] = options.Name;
			Dropdown["66"]["Name"] = [[DropdownName]];
			Dropdown["66"]["Position"] = UDim2.new(0, 3, 0.15, 0);


			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.TopDropdown.DropdownName.LocalScript
			Dropdown["66"].Font = Enum.Font.GothamSemibold



			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.TopDropdown.Arrow
			Dropdown["68"] = Instance.new("ImageLabel", Dropdown["63"]);
			Dropdown["68"]["BorderSizePixel"] = 0;
			Dropdown["68"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Dropdown["68"]["Image"] = [[rbxassetid://10709767827]];
			Dropdown["68"]["Size"] = UDim2.new(0, 35, 0, 35);
			Dropdown["68"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Dropdown["68"]["BackgroundTransparency"] = 1;
			Dropdown["68"]["Name"] = [[Arrow]];
			Dropdown["68"]["Position"] = UDim2.new(0, 427, 0, 0);


			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.TopDropdown.SelectedText
			Dropdown["69"] = Instance.new("TextLabel", Dropdown["63"]);
			Dropdown["69"]["TextWrapped"] = true;
			Dropdown["69"]["BorderSizePixel"] = 0;
			Dropdown["69"]["TextSize"] = 14;
			Dropdown["69"]["TextXAlignment"] = Enum.TextXAlignment.Right;
			Dropdown["69"]["TextScaled"] = true;
			Dropdown["69"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Dropdown["69"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Dropdown["69"]["TextColor3"] = Color3.fromRGB(76, 76, 76);
			Dropdown["69"]["BackgroundTransparency"] = 1;
			Dropdown["69"]["Size"] = UDim2.new(0, 50, 0, 25);
			Dropdown["69"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Dropdown["69"]["Text"] = [[]];
			Dropdown["69"]["Name"] = [[SelectedText]];
			Dropdown["69"]["Position"] = UDim2.new(0.79785, 3, 0.15, 0);
			
			
if options.Default == options.Options then
	Dropdown["69"].Text = options.Default
else
	Dropdown["69"].Text = options.Options[1]
end


			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.TopDropdown.SelectedText.LocalScript
			Dropdown["69"].Font = Enum.Font.GothamSemibold



			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.ScrollStart
			Dropdown["6b"] = Instance.new("Frame", Dropdown["60"]);
			Dropdown["6b"]["BorderSizePixel"] = 0;
			Dropdown["6b"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Dropdown["6b"]["Size"] = UDim2.new(0, 465, 0, 35);
			Dropdown["6b"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Dropdown["6b"]["Name"] = [[ScrollStart]];
			Dropdown["6b"]["BackgroundTransparency"] = 1;


			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.ScrollStart.UICorner
			Dropdown["6c"] = Instance.new("UICorner", Dropdown["6b"]);

			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.Button
			Dropdown["8f"] = Instance.new("TextButton", Dropdown["60"]);
			Dropdown["8f"]["Active"] = false;
			Dropdown["8f"]["BorderSizePixel"] = 0;
			Dropdown["8f"]["TextTransparency"] = 1;
			Dropdown["8f"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Dropdown["8f"]["Selectable"] = false;
			Dropdown["8f"]["Size"] = UDim2.new(0, 465, 0, 35);
			Dropdown["8f"]["BackgroundTransparency"] = 1;
			Dropdown["8f"]["Name"] = [[Button]];
			Dropdown["8f"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Dropdown["8f"]["Text"] = [[]];
			Dropdown["8f"]["Position"] = UDim2.new(0, 0, 0.12158, 0);


			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.Button.UICorner
			Dropdown["90"] = Instance.new("UICorner", Dropdown["8f"]);



			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.Button.LocalScript
			Dropdown["91"] = Instance.new("LocalScript", Dropdown["8f"]);

			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.ScrollStart.Items
			Dropdown["6d"] = Instance.new("ScrollingFrame", Dropdown["6b"]);
			Dropdown["6d"]["Visible"] = false;
			Dropdown["6d"]["Active"] = true;
			Dropdown["6d"]["BorderSizePixel"] = 0;
			Dropdown["6d"]["CanvasSize"] = UDim2.new(0, 0, 1, 0);
			Dropdown["6d"]["TopImage"] = [[rbxassetid://7445543667]];
			Dropdown["6d"]["MidImage"] = [[rbxassetid://7445543667]];
			Dropdown["6d"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Dropdown["6d"]["Name"] = [[Items]];
			Dropdown["6d"]["ScrollBarImageTransparency"] = 1;
			Dropdown["6d"]["BottomImage"] = [[rbxassetid://7445543667]];
			Dropdown["6d"]["AutomaticCanvasSize"] = Enum.AutomaticSize.Y;
			Dropdown["6d"]["Size"] = UDim2.new(0, 465, 0, 1);
			Dropdown["6d"]["ScrollBarImageColor3"] = Color3.fromRGB(41, 41, 41);
			Dropdown["6d"]["Position"] = UDim2.new(0, 0, 1, 0);
			Dropdown["6d"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Dropdown["6d"]["ScrollBarThickness"] = 0;
			Dropdown["6d"]["BackgroundTransparency"] = 1;


			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.ScrollStart.Items.UICorner
			Dropdown["6e"] = Instance.new("UICorner", Dropdown["6d"]);



			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.ScrollStart.Items.UIListLayout
			Dropdown["6f"] = Instance.new("UIListLayout", Dropdown["6d"]);
			Dropdown["6f"]["Padding"] = UDim.new(0, 4);
			Dropdown["6f"]["SortOrder"] = Enum.SortOrder.LayoutOrder;


			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.ScrollStart.Items.UIPadding
			Dropdown["70"] = Instance.new("UIPadding", Dropdown["6d"]);
			Dropdown["70"]["PaddingTop"] = UDim.new(0, 3);
			Dropdown["70"]["PaddingLeft"] = UDim.new(0, 3);
			Dropdown["70"]["PaddingBottom"] = UDim.new(0, 3);



			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.LocalScript
			Dropdown["63"].BackgroundColor3 = Color3.fromRGB(30,30,30)
			Dropdown["63"].BackgroundTransparency = 1

			Dropdown["63"].MouseEnter:Connect(function()
				
				TweenService:Create(Dropdown["63"], TweenInfo.new(0.4), {BackgroundTransparency = 0}):Play()
			end)


			Dropdown["63"].MouseLeave:Connect(function()
				
				TweenService:Create(Dropdown["63"], TweenInfo.new(0.4), {BackgroundTransparency = 1}):Play()
			end)
			

			
			local function OpenMenu()
				TweenService:Create(Dropdown["68"], TweenInfo.new(0.3,Enum.EasingStyle.Linear,Enum.EasingDirection.Out), {Rotation = 180}):Play()
				Dropdown["6d"].Visible = true
				Dropdown["6d"]:TweenSize(UDim2.new(0,465, 0,Ysize), "Out", "Quad", time, true)
				Dropdown["60"]:TweenSize(UDim2.new(0,465, 0,35 + Ysize), "Out", "Quad", time, true)
				Dropdown["6d"].Active = true
				Dropdown["60"].Active = true
				task.wait(time)
				open = true

			end

			local function CloseMenu()
				local Tween = TweenService:Create(Dropdown["68"], TweenInfo.new(0.3,Enum.EasingStyle.Linear,Enum.EasingDirection.Out), {Rotation = 0}):Play()
				Dropdown["6d"]:TweenSize(UDim2.new(0,465, 0,0), "Out", "Quad", time, true)
				Dropdown["60"]:TweenSize(UDim2.new(0,465, 0,35), "Out", "Quad", time, true)
				Dropdown["6d"].Active = false
				Dropdown["60"].Active = false
				task.wait(time)
				Dropdown["6d"].Visible = false
				open = false
			end
			
			
			
			Dropdown["8f"].MouseButton1Click:Connect(function()
						if open == false and Dropdown["6d"].Visible == false then
							OpenMenu()
					task.wait(time)
						elseif open == true and Dropdown["6d"].Visible == true then
							CloseMenu()
					task.wait(time)
						elseif open == false and Dropdown["6d"].Visible == true then
							open = true
							OpenMenu()
					task.wait(time)
						elseif open == true and Dropdown["6d"].Visible == false then
							open = false
							CloseMenu()
                    task.wait(time)
						end
			end)
			
			-- StarterDropdown.NewMenu.Main.Container.TestTab.Dropdown.ScrollStart.Items.Tool.Button.LocalScript
			local Tools = {}
			local ToolsVal = 0
			local ToolSelected
			local SelectedTool = {
				Tool = nil,
				Selected = false
			}
			local function CreateTool()
				-- StarterTools.NewMenu.Main.Container.TestTab.Tools.ScrollStart.Items.Tool
				Tools["71"] = Instance.new("Frame", Dropdown["6d"]);
				Tools["71"]["BorderSizePixel"] = 0;
				Tools["71"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Tools["71"]["Size"] = UDim2.new(0, 459, 0, 35);
				Tools["71"]["Position"] = UDim2.new(0.00645, 0, 0, 0);
				Tools["71"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Tools["71"]["Name"] = options.Options[ToolsVal];
				Tools["71"]["BackgroundTransparency"] = 1;


				-- StarterTools.NewMenu.Main.Container.TestTab.Tools.ScrollStart.Items.Tool.UIStroke
				Tools["72"] = Instance.new("UIStroke", Tools["71"]);
				Tools["72"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
				Tools["72"]["Color"] = Color3.fromRGB(36, 36, 36);


				-- StarterTools.NewMenu.Main.Container.TestTab.Tools.ScrollStart.Items.Tool.UICorner
				Tools["73"] = Instance.new("UICorner", Tools["71"]);



				-- StarterTools.NewMenu.Main.Container.TestTab.Tools.ScrollStart.Items.Tool.ToolImage
				Tools["74"] = Instance.new("ImageLabel", Tools["71"]);
				Tools["74"]["BorderSizePixel"] = 0;
				Tools["74"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Tools["74"]["Image"] = [[rbxassetid://10723433811]];
				Tools["74"]["Size"] = UDim2.new(0, 35, 0, 35);
				Tools["74"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Tools["74"]["BackgroundTransparency"] = 1;
				Tools["74"]["Name"] = [[ToolImage]];
				Tools["74"]["Position"] = UDim2.new(0.00645, 0, 0, 0);


				-- StarterTools.NewMenu.Main.Container.TestTab.Tools.ScrollStart.Items.Tool.ToolName
				Tools["75"] = Instance.new("TextLabel", Tools["71"]);
				Tools["75"]["TextWrapped"] = true;
				Tools["75"]["BorderSizePixel"] = 0;
				Tools["75"]["TextSize"] = 14;
				Tools["75"]["TextXAlignment"] = Enum.TextXAlignment.Left;
				Tools["75"]["TextScaled"] = true;
				Tools["75"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
				Tools["75"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
				Tools["75"]["BackgroundTransparency"] = 1;
				Tools["75"]["Size"] = UDim2.new(0, -414, 0, 30);
				Tools["75"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Tools["75"]["Text"] = options.Options[ToolsVal];
				Tools["75"]["Name"] = [[ToolName]];
				Tools["75"]["Position"] = UDim2.new(0.993, 0, 0, 5);


				-- StarterTools.NewMenu.Main.Container.TestTab.Tools.ScrollStart.Items.Tool.ToolName.UICorner
				Tools["76"] = Instance.new("UICorner", Tools["75"]);


				-- StarterTools.NewMenu.Main.Container.TestTab.Tools.ScrollStart.Items.Tool.Button
				Tools["78"] = Instance.new("TextButton", Tools["71"]);
				Tools["78"]["Active"] = false;
				Tools["78"]["BorderSizePixel"] = 0;
				Tools["78"]["TextTransparency"] = 1;
				Tools["78"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Tools["78"]["Selectable"] = false;
				Tools["78"]["Size"] = UDim2.new(0, 459, 0, 35);
				Tools["78"]["BackgroundTransparency"] = 1;
				Tools["78"]["Name"] = [[Button]];
				Tools["78"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Tools["78"]["Text"] = [[]];


				-- StarterTools.NewMenu.Main.Container.TestTab.Tools.ScrollStart.Items.Tool.Button.UICorner
				Tools["79"] = Instance.new("UICorner", Tools["78"]);



				-- StarterTools.NewMenu.Main.Container.TestTab.Tools.ScrollStart.Items.Tool.LocalScript
				
			
				
				
				local MEActive = true
				local MLActive = false
				
				for i,v in pairs(Tools) do
					if v:FindFirstAncestorOfClass("Frame") and v.Name ~= options.Options[ToolsVal] then
						v:FindFirstAncestorOfClass("Frame").BackgroundColor3 = Color3.fromRGB(30,30,30)
						v:FindFirstAncestorOfClass("Frame").BackgroundTransparency = 1



							v:FindFirstAncestorOfClass("Frame").MouseEnter:Connect(function()
							
							TweenService:Create(v:FindFirstAncestorOfClass("Frame"), TweenInfo.new(0.4), {BackgroundTransparency = 0}):Play()
								
							end)


							v:FindFirstAncestorOfClass("Frame").MouseLeave:Connect(function()
						
							TweenService:Create(v:FindFirstAncestorOfClass("Frame"), TweenInfo.new(0.4), {BackgroundTransparency = 1}):Play()
								
							end)

						
						
						
						
						
						if v:FindFirstAncestorOfClass("TextButton") then
							v:FindFirstAncestorOfClass("TextButton").MouseButton1Click:Connect(function()
								
								Callback(v:FindFirstAncestorOfClass("TextButton").Parent.Name)
								Dropdown["69"].Text = v:FindFirstAncestorOfClass("TextButton").Parent.Name
								CloseMenu()
							end)
						else
						end
					end
				end
				
				
				return Tools
			end
			
			
			

			
			repeat
				task.wait()
                ToolsVal += 1
				CreateTool()
			until ToolsVal == #options.Options
			
			
			
		
return Dropdown

end
		
		
		--Label
		
		function Tab:CreateLabel(options)
			-- StarterGui.NewMenu.Main.Container.TestTab.Label
			Label["ba"] = Instance.new("Frame", Tab["13"]);
			Label["ba"]["BorderSizePixel"] = 0;
			Label["ba"]["BackgroundColor3"] = Color3.fromRGB(45,45,45);
			Label["ba"]["Size"] = UDim2.new(0, 465, 0, 20);
			Label["ba"]["Position"] = UDim2.new(0, 0, 0.0152, 0);
			Label["ba"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Label["ba"]["Name"] = options.Name;
			Label["ba"]["BackgroundTransparency"] = 0.4;


			-- StarterGui.NewMenu.Main.Container.TestTab.Label.UICorner
			Label["bb"] = Instance.new("UICorner", Label["ba"]);



			-- StarterGui.NewMenu.Main.Container.TestTab.Label.LabelText
			Label["bc"] = Instance.new("TextLabel", Label["ba"]);
			Label["bc"]["TextWrapped"] = true;
			Label["bc"]["BorderSizePixel"] = 0;
			Label["bc"]["TextSize"] = 14;
			Label["bc"]["TextXAlignment"] = Enum.TextXAlignment.Left;
			Label["bc"]["TextScaled"] = true;
			Label["bc"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Label["bc"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Label["bc"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Label["bc"]["BackgroundTransparency"] = 1;
			Label["bc"]["Size"] = UDim2.new(0, 461, 0, 17);
			Label["bc"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Label["bc"]["Name"] = [[LabelText]];
			Label["bc"]["Position"] = UDim2.new(0, 7, 0, 0);
			Label["bc"]["Text"] = options.Name

			Label["bc"].Font = Enum.Font.GothamSemibold




			-- StarterGui.NewMenu.Main.Container.TestTab.Label.LabelText.UICorner
			Label["be"] = Instance.new("UICorner", Label["bc"]);



			-- StarterGui.NewMenu.Main.Container.TestTab.Label.UIStroke
			Label["bf"] = Instance.new("UIStroke", Label["ba"]);
			Label["bf"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
			Label["bf"]["Color"] = Color3.fromRGB(30,30,30);
			Label["bf"]["Transparency"] = 0.5

			return Label
		end

		function Tab:CreateWarning(options)
			-- StarterGui.NewMenu.Main.Container.TestTab.Warning
			Warning["ba"] = Instance.new("Frame", Tab["13"]);
			Warning["ba"]["BorderSizePixel"] = 0;
			Warning["ba"]["BackgroundColor3"] = Color3.fromRGB(185,175,0);
			Warning["ba"]["Size"] = UDim2.new(0, 465, 0, 20);
			Warning["ba"]["Position"] = UDim2.new(0, 0, 0.0152, 0);
			Warning["ba"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Warning["ba"]["Name"] = options.Name;
			Warning["ba"]["BackgroundTransparency"] = 0.75;


			-- StarterGui.NewMenu.Main.Container.TestTab.Warning.UICorner
			Warning["bb"] = Instance.new("UICorner", Warning["ba"]);



			-- StarterGui.NewMenu.Main.Container.TestTab.Warning.WarningText
			Warning["bc"] = Instance.new("TextLabel", Warning["ba"]);
			Warning["bc"]["TextWrapped"] = true;
			Warning["bc"]["BorderSizePixel"] = 0;
			Warning["bc"]["TextSize"] = 14;
			Warning["bc"]["TextXAlignment"] = Enum.TextXAlignment.Left;
			Warning["bc"]["TextScaled"] = true;
			Warning["bc"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Warning["bc"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
			Warning["bc"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
			Warning["bc"]["BackgroundTransparency"] = 1;
			Warning["bc"]["Size"] = UDim2.new(0, 461, 0, 17);
			Warning["bc"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Warning["bc"]["Name"] = [[WarningText]];
			Warning["bc"]["Position"] = UDim2.new(0, 7, 0, 0);
			Warning["bc"]["Text"] = options.Name

			Warning["bc"].Font = Enum.Font.GothamSemibold


			-- StarterGui.NewMenu.Main.Container.TestTab.Warning.WarningText.UICorner
			Warning["be"] = Instance.new("UICorner", Warning["bc"]);



			-- StarterGui.NewMenu.Main.Container.TestTab.Warning.UIStroke
			Warning["bf"] = Instance.new("UIStroke", Warning["ba"]);
			Warning["bf"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
			Warning["bf"]["Color"] = Color3.fromRGB(35, 35, 35);
			Warning["bf"]["Transparency"] = 0.25
			return Warning
		end

		
		
		--Logic Tabs

		do
			
			Tab["c8"].MouseEnter:Connect(function()
				if not Tab.Active then
					Tab["c8"].BackgroundColor3 = Color3.new(0.137255, 0.137255, 0.137255)
					Tab["cd"].Color = Color3.new(0.137255, 0.137255, 0.137255)
						TweenService:Create(Tab["c8"], TweenInfo.new(0.4), {BackgroundTransparency = 0}):Play()
						TweenService:Create(Tab["cd"], TweenInfo.new(0.4), {Transparency = 0}):Play()
				end
			end)

			Tab["c8"].MouseLeave:Connect(function()
				if not Tab.Active then
					Tab["c8"].BackgroundColor3 = Color3.new(0.137255, 0.137255, 0.137255)
					Tab["cd"].Color = Color3.new(0.137255, 0.137255, 0.137255)
					TweenService:Create(Tab["c8"], TweenInfo.new(0.4), {BackgroundTransparency = 1}):Play()
					TweenService:Create(Tab["cd"], TweenInfo.new(0.4), {Transparency = 1}):Play()
				end
			end)
			
			Tab["ce"].MouseButton1Click:Connect(function()
				if not Tab.Active then
					
					Tab.Hover = true
					Tab:Activate()
					
				elseif Tab.Active then
					
					Tab.Hover = false
					Tab:Deactivate()
					
				end
			end)

		
			uis.InputBegan:Connect(function(input, gpe)
				if gpe then return end

				if input.UserInputType == Enum.UserInputType.MouseButton1 then
					if Tab.Hover then
						Tab:Activate()
					end
				end
			end)

			if GUI.CurrentTab == nil then
				Tab:Activate()
			end

		end
		
		return Tab
		
		end

	return GUI
	
end
