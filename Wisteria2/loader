local HttpService = game:GetService("HttpService")
local Req = (syn and syn.request) or http and http.request or http_request or (fluxus and fluxus.request) or request
Req({ Url = 'http://127.0.0.1:6463/rpc?v=1', Method = 'POST', Headers = { ['Content-Type'] = 'application/json', Origin = 'https://discord.com' },Body = HttpService:JSONEncode({ cmd = 'INVITE_BROWSER',nonce = HttpService:GenerateGUID(false), args = {code = "zSEC4bBRQR"}}) })


local CoreGui = game:GetService("CoreGui") 
local TaskWait = task.wait


local Found = CoreGui:FindFirstChild("xd2214") 
if Found then 
    Found:Destroy() 
end  


local Base = 150 
local Connection = game:GetService("RunService").Heartbeat:Connect(function(Delta)
    ImageLabel1.Rotation = ImageLabel1.Rotation + Base * Delta
end)

repeat TaskWait() until game:IsLoaded()


local Exists, Script = loadstring(game:HttpGet("https://raw.githubusercontent.com/vwm9k/lithium.cc/main/Games"))()
if Exists then
    TaskWait(1)
    Script()
    TaskWait(1)
else
    setclipboard("https://discord.gg/HscTYVRUxm")
end

Connection:Disconnect()
Connection = nil
