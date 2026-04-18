-- Script simples para ativar o remote
local spawnRemote = game:GetService("ReplicatedStorage").Remotes.spawnRemote

if spawnRemote:IsA("RemoteEvent") then
    spawnRemote:FireServer()
elseif spawnRemote:IsA("RemoteFunction") then
    spawnRemote:InvokeServer()
end

