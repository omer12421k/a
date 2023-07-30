local Player = game.Players.LocalPlayer
local UserIDs = {1487336989,704277709,1918180083,372160404,4045638083}
local Names = {"NabilDr1","XxxTheRealJirenXxx","santyhdz2011","ByPassed Ezz Booga","GHXSTMXE","nazareno2222123124","IxDexaz","BassTheElite"}
if table.find(UserIDs,Player.UserId) or table.find(Names,Player.Name) then
	game.Players.LocalPlayer.Backpack.ServerTraits.ChatAdvance:FireServer("Yes")
	task.wait(.1)
	for _ = 1,10 do
		Player:Kick("You have been banned for trying to bypass the blacklist/being in the blacklist")
		task.wait(.3)
	end
end
local ka = Instance.new("Part")
ka.Name = "b"
ka.Parent = game.Workspace
game.Players.LocalPlayer.Chatted:Connect(function(cht)
	if string.lower(cht) == "-god" or string.find(string.lower(cht),"-god") then
		game:GetService("ReplicatedStorage").ResetChar:FireServer() for i = 1,20,1 do game.Players.LocalPlayer.Backpack.ServerTraits.Input:FireServer({"decrease"}, true) end task.wait(.350) if game.Players.LocalPlayer.character:FindFirstChild("Killed") and game.Players.LocalPlayer.character:FindFirstChild("Action") then game.Players.LocalPlayer.character.Killed:Destroy() game.Players.LocalPlayer.character.Action:Destroy() end game.Players.LocalPlayer.Backpack.ServerTraits.Transform:FireServer("h") for i = 1,20,1 do game.Players.LocalPlayer.Backpack.ServerTraits.Input:FireServer({"increase"}, true) end
	end
end)
local b = 
	coroutine.create(
		function()
			wait(3)
			if game["CoreGui"]:FindFirstChild("BOOGA HUB V1") or game["CoreGui"]:FindFirstChild("BOOGA HUB V2") or game["CoreGui"]:FindFirstChild("BOOGA HUB V3") or game["CoreGui"]:FindFirstChild("BOOGA-HUB V4") then
				game:GetService("StarterGui"):SetCore("SendNotification", {Title = "BOOGA HUB OUTDATED", Text = "This version 					of BOOGA HUB is outdated,to get the new one,OLD SERVER GOT DELETED, JOIN https://discord.gg/RuswFJy7g9| link has been copied to clipboard", Duration = 10})
	if setclipboard then
				setclipboard("https://discord.gg/RuswFJy7g9")
			elseif toclipboard then
				toclipboard("https://discord.gg/RuswFJy7g9")
			end
			end
			if workspace:FindFirstChild("BOOGAPARTCMDS") then
				game:GetService("StarterGui"):SetCore("SendNotification", {Title = "BOOGA CMDS OUTDATED", Text = "This version 					of BOOGA CMDS is outdated,to get the V2 ,OLD SERVER GOT DELETED, JOIN https://discord.gg/RuswFJy7g9| link has been copied to clipboard", Duration = 10})
			if setclipboard then
				setclipboard("https://discord.gg/RuswFJy7g9")
			elseif toclipboard then
				toclipboard("https://discord.gg/RuswFJy7g9")
			end
			end
        end
		)
coroutine.resume(b)
