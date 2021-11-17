

NANE = "POWER X HUB|BLOX FRUIT 4.2"

if game.CoreGui:FindFirstChild(NANE) then
    game.CoreGui:FindFirstChild(NANE):Destroy()
end

local Heeee = loadstring(game:HttpGet("https://raw.githubusercontent.com/MASTERHUB2/POWER-X-UI/main/README.md"))() --someone reuploaded it so I put it in place of the original back up so guy can get free credit.
local powerx = Heeee.new(NANE, 5013109572)

-- themes
local themes = {
Background = Color3.fromRGB(24, 24, 24),
Glow = Color3.fromRGB(0, 0, 0),
Accent = Color3.fromRGB(10, 10, 10),
LightContrast = Color3.fromRGB(20, 20, 20),
DarkContrast = Color3.fromRGB(14, 14, 14),  
TextColor = Color3.fromRGB(0, 255, 255)
}


local OldWorld = false
local Sea2 = false
local ThreeWorld = false
local placeId = game.PlaceId
if placeId == 2753915549 then
   OldWorld = true
elseif placeId == 4442272183 then
   Sea2 = true
elseif placeId == 7449423635 then
   ThreeWorld = true
end

if Sea2 then
   for i,v in pairs(game:GetService("ReplicatedStorage"):GetDescendants()) do
      if v.Name == "DarkBlade" then
         v.Parent.Name = "NoobRip"
      end
   end
end
if OldWorld then
   for i,v in pairs(game:GetService("ReplicatedStorage"):GetDescendants()) do
      if v.Name == "XavierWoods_HairAccessory" then
         v.Parent.Name = "NoobRipIndra"
      end
   end
end
if not game:GetService("UserInputService").TouchEnabled and not game:GetService("UserInputService").KeyboardEnabled == false then
   _G.bringmob = true
end

function CheckQuest()
   local MyLevel = game.Players.localPlayer.Data.Level.Value
   if OldWorld then
      if MyLevel == 1 or MyLevel <= 9 then -- Bandit
         Ms = "Bandit [Lv. 5]"
         QuestName = "BanditQuest1"
         LevelQuest = 1
         NameMon = "Bandit"
         CFrameQuest = CFrame.new(1061.66699, 16.5166187, 1544.52905, -0.942978859, -3.33851502e-09, 0.332852632, 7.04340497e-09, 1, 2.99841325e-08, -0.332852632, 3.06188177e-08, -0.942978859)
         CFrameMon = CFrame.new(1199.31287, 52.2717781, 1536.91516, -0.929782331, 6.60215846e-08, -0.368109822, 3.9077392e-08, 1, 8.06501603e-08, 0.368109822, 6.06023249e-08, -0.929782331)
      elseif MyLevel == 10 or MyLevel <= 14 then -- Monkey
         Ms = "Monkey [Lv. 14]"
         QuestName = "JungleQuest"
         LevelQuest = 1
         NameMon = "Monkey"
         CFrameQuest = CFrame.new(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
         CFrameMon = CFrame.new(-1402.74609, 98.5633316, 90.6417007, 0.836947978, 0, 0.547282517, -0, 1, -0, -0.547282517, 0, 0.836947978)
      elseif MyLevel == 15 or MyLevel <= 29 then -- Gorilla
         Ms = "Gorilla [Lv. 20]"
         QuestName = "JungleQuest"
         LevelQuest = 2
         NameMon = "Gorilla"
         CFrameQuest = CFrame.new(-1604.12012, 36.8521118, 154.23732, 0.0648873374, -4.70858913e-06, -0.997892559, 1.41431883e-07, 1, -4.70933674e-06, 0.997892559, 1.64442184e-07, 0.0648873374)
         CFrameMon = CFrame.new(-1223.52808, 6.27936459, -502.292664, 0.310949147, -5.66602516e-08, 0.950426519, -3.37275488e-08, 1, 7.06501808e-08, -0.950426519, -5.40241736e-08, 0.310949147)
      elseif MyLevel == 30 or MyLevel <= 39 then -- Pirate
         Ms = "Pirate [Lv. 35]"
         QuestName = "BuggyQuest1"
         LevelQuest = 1
         NameMon = "Pirate"
         CFrameQuest = CFrame.new(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
         CFrameMon = CFrame.new(-1219.32324, 4.75205183, 3915.63452, -0.966492832, -6.91238853e-08, 0.25669381, -5.21195496e-08, 1, 7.3047012e-08, -0.25669381, 5.72206496e-08, -0.966492832)
      elseif MyLevel == 40 or MyLevel <= 59 then -- Brute
         Ms = "Brute [Lv. 45]"
         QuestName = "BuggyQuest1"
         LevelQuest = 2
         NameMon = "Brute"
         CFrameQuest = CFrame.new(-1139.59717, 4.75205183, 3825.16211, -0.959730506, -7.5857054e-09, 0.280922383, -4.06310328e-08, 1, -1.11807175e-07, -0.280922383, -1.18718916e-07, -0.959730506)
         CFrameMon = CFrame.new(-1146.49646, 96.0936813, 4312.1333, -0.978175163, -1.53222057e-08, 0.207781896, -3.33316912e-08, 1, -8.31738873e-08, -0.207781896, -8.82843523e-08, -0.978175163)
      elseif MyLevel == 60 or MyLevel <= 74 then -- Desert Bandit
         Ms = "Desert Bandit [Lv. 60]"
         QuestName = "DesertQuest"
         LevelQuest = 1
         NameMon = "Desert Bandit"
         CFrameQuest = CFrame.new(897.031128, 6.43846416, 4388.97168, -0.804044724, 3.68233266e-08, 0.594568789, 6.97835176e-08, 1, 3.24365246e-08, -0.594568789, 6.75715199e-08, -0.804044724)
         CFrameMon = CFrame.new(932.788818, 6.4503746, 4488.24609, -0.998625934, 3.08948351e-08, 0.0524050146, 2.79967303e-08, 1, -5.60361286e-08, -0.0524050146, -5.44919629e-08, -0.998625934)
      elseif MyLevel == 75 or MyLevel <= 89 then -- Desert Officre
         Ms = "Desert Officer [Lv. 70]"
         QuestName = "DesertQuest"
         LevelQuest = 2
         NameMon = "Desert Officer"
         CFrameQuest = CFrame.new(897.031128, 6.43846416, 4388.97168, -0.804044724, 3.68233266e-08, 0.594568789, 6.97835176e-08, 1, 3.24365246e-08, -0.594568789, 6.75715199e-08, -0.804044724)
         CFrameMon = CFrame.new(1580.03198, 4.61375761, 4366.86426, 0.135744005, -6.44280718e-08, -0.990743816, 4.35738308e-08, 1, -5.90598574e-08, 0.990743816, -3.51534837e-08, 0.135744005)
      elseif MyLevel == 90 or MyLevel <= 99 then -- Snow Bandits
         Ms = "Snow Bandit [Lv. 90]"
         QuestName = "SnowQuest"
         LevelQuest = 1
         NameMon = "Snow Bandits"
         CFrameQuest = CFrame.new(1384.14001, 87.272789, -1297.06482, 0.348555952, -2.53947841e-09, -0.937287986, 1.49860568e-08, 1, 2.86358204e-09, 0.937287986, -1.50443711e-08, 0.348555952)
         CFrameMon = CFrame.new(1370.24316, 102.403511, -1411.52905, 0.980274439, -1.12995728e-08, 0.197641045, -9.57343449e-09, 1, 1.04655214e-07, -0.197641045, -1.04482936e-07, 0.980274439)
      elseif MyLevel == 100 or MyLevel <= 119 then -- Snowman
         Ms = "Snowman [Lv. 100]"
         QuestName = "SnowQuest"
         LevelQuest = 2
         NameMon = "Snowman"
         CFrameQuest = CFrame.new(1384.14001, 87.272789, -1297.06482, 0.348555952, -2.53947841e-09, -0.937287986, 1.49860568e-08, 1, 2.86358204e-09, 0.937287986, -1.50443711e-08, 0.348555952)
         CFrameMon = CFrame.new(1370.24316, 102.403511, -1411.52905, 0.980274439, -1.12995728e-08, 0.197641045, -9.57343449e-09, 1, 1.04655214e-07, -0.197641045, -1.04482936e-07, 0.980274439)
      elseif MyLevel == 120 or MyLevel <= 149 then -- Chief Petty Officer
         Ms = "Chief Petty Officer [Lv. 120]"
         QuestName = "MarineQuest2"
         LevelQuest = 1
         NameMon = "Chief Petty Officer"
         CFrameQuest = CFrame.new(-5035.0835, 28.6520386, 4325.29443, 0.0243340395, -7.08064647e-08, 0.999703884, -6.36926814e-08, 1, 7.23777944e-08, -0.999703884, -6.54350671e-08, 0.0243340395)
         CFrameMon = CFrame.new(-4882.8623, 22.6520386, 4255.53516, 0.273695946, -5.40380647e-08, -0.96181643, 4.37720793e-08, 1, -4.37274998e-08, 0.96181643, -3.01326679e-08, 0.273695946)
      elseif MyLevel == 150 or MyLevel <= 174 then -- Sky Bandit
         Ms = "Sky Bandit [Lv. 150]"
         QuestName = "SkyQuest"
         LevelQuest = 1
         NameMon = "Sky Bandit"
         CFrameQuest = CFrame.new(-4841.83447, 717.669617, -2623.96436, -0.875942111, 5.59710216e-08, -0.482416272, 3.04023082e-08, 1, 6.08195947e-08, 0.482416272, 3.86078725e-08, -0.875942111)
         CFrameMon = CFrame.new(-4970.74219, 294.544342, -2890.11353, -0.994874597, -8.61311236e-08, -0.101116329, -9.10836206e-08, 1, 4.43614923e-08, 0.101116329, 5.33441664e-08, -0.994874597)
      elseif MyLevel == 175 or MyLevel <= 224 then -- Dark Master
         Ms = "Dark Master [Lv. 175]"
         QuestName = "SkyQuest"
         LevelQuest = 2
         NameMon = "Dark Master"
         CFrameQuest = CFrame.new(-4841.83447, 717.669617, -2623.96436, -0.875942111, 5.59710216e-08, -0.482416272, 3.04023082e-08, 1, 6.08195947e-08, 0.482416272, 3.86078725e-08, -0.875942111)
         CFrameMon = CFrame.new(-5220.58594, 430.693298, -2278.17456, -0.925375521, 1.12086873e-08, 0.379051805, -1.05115507e-08, 1, -5.52320891e-08, -0.379051805, -5.50948407e-08, -0.925375521)
      elseif MyLevel == 225 or MyLevel <= 274 then -- Toga Warrior
         Ms = "Toga Warrior [Lv. 225]"
         QuestName = "ColosseumQuest"
         LevelQuest = 1
         NameMon = "Toga Warrior"
         CFrameQuest = CFrame.new(-1576.11743, 7.38933945, -2983.30762, 0.576966345, 1.22114863e-09, 0.816767931, -3.58496594e-10, 1, -1.24185606e-09, -0.816767931, 4.2370063e-10, 0.576966345)
         CFrameMon = CFrame.new(-1779.97583, 44.6077499, -2736.35474, 0.984437346, 4.10396339e-08, 0.175734788, -3.62286876e-08, 1, -3.05844168e-08, -0.175734788, 2.3741821e-08, 0.984437346)
      elseif MyLevel == 275 or MyLevel <= 299 then -- Gladiato
         Ms = "Gladiator [Lv. 275]"
         QuestName = "ColosseumQuest"
         LevelQuest = 2
         NameMon = "Gladiato"
         CFrameQuest = CFrame.new(-1576.11743, 7.38933945, -2983.30762, 0.576966345, 1.22114863e-09, 0.816767931, -3.58496594e-10, 1, -1.24185606e-09, -0.816767931, 4.2370063e-10, 0.576966345)
         CFrameMon = CFrame.new(-1274.75903, 58.1895943, -3188.16309, 0.464524001, 6.21005611e-08, 0.885560572, -4.80449414e-09, 1, -6.76054768e-08, -0.885560572, 2.71497012e-08, 0.464524001)
      elseif MyLevel == 300 or MyLevel <= 329 then -- Military Soldier
         Ms = "Military Soldier [Lv. 300]"
         QuestName = "MagmaQuest"
         LevelQuest = 1
         NameMon = "Military Soldier"
         CFrameQuest = CFrame.new(-5316.55859, 12.2370615, 8517.2998, 0.588437557, -1.37880001e-08, -0.808542669, -2.10116209e-08, 1, -3.23446478e-08, 0.808542669, 3.60215964e-08, 0.588437557)
         CFrameMon = CFrame.new(-5363.01123, 41.5056877, 8548.47266, -0.578253984, -3.29503091e-10, 0.815856814, 9.11209668e-08, 1, 6.498761e-08, -0.815856814, 1.11920997e-07, -0.578253984)
      elseif MyLevel == 300 or MyLevel <= 374 then -- Military Spy
         Ms = "Military Spy [Lv. 330]"
         QuestName = "MagmaQuest"
         LevelQuest = 2
         NameMon = "Military Spy"
         CFrameQuest = CFrame.new(-5316.55859, 12.2370615, 8517.2998, 0.588437557, -1.37880001e-08, -0.808542669, -2.10116209e-08, 1, -3.23446478e-08, 0.808542669, 3.60215964e-08, 0.588437557)
         CFrameMon = CFrame.new(-5787.99023, 120.864456, 8762.25293, -0.188358366, -1.84706277e-08, 0.982100308, -1.23782129e-07, 1, -4.93306951e-09, -0.982100308, -1.22495649e-07, -0.188358366)
      elseif MyLevel == 375 or MyLevel <= 399 then -- Fishman Warrior 
         Ms = "Fishman Warrior [Lv. 375]"
         QuestName = "FishmanQuest"
         LevelQuest = 1
         NameMon = "Fishman Warrior"
         CFrameQuest = CFrame.new(61122.65234375, 18.497442245483, 1569.3997802734)
         CFrameMon = CFrame.new(60844.10546875, 98.462875366211, 1298.3985595703)
      elseif MyLevel == 400 or MyLevel <= 449 then -- Fishman Commando
         Ms = "Fishman Commando [Lv. 400]"
         QuestName = "FishmanQuest"
         LevelQuest = 2
         NameMon = "Fishman Commando"
         CFrameQuest = CFrame.new(61122.65234375, 18.497442245483, 1569.3997802734)
         CFrameMon = CFrame.new(61738.3984375, 64.207321166992, 1433.8375244141)
      elseif MyLevel == 450 or MyLevel <= 474 then -- God's Guards
         Ms = "God's Guard [Lv. 450]"
         QuestName = "SkyExp1Quest"
         LevelQuest = 1
         NameMon = "God's Guards"
         CFrameQuest = CFrame.new(-4721.71436, 845.277161, -1954.20105, -0.999277651, -5.56969759e-09, 0.0380011722, -4.14751478e-09, 1, 3.75035256e-08, -0.0380011722, 3.73188307e-08, -0.999277651)
         CFrameMon = CFrame.new(-4716.95703, 853.089722, -1933.92542, -0.93441087, -6.77488776e-09, -0.356197298, 1.12145182e-08, 1, -4.84390199e-08, 0.356197298, -4.92565206e-08, -0.93441087)
      elseif MyLevel == 475 or MyLevel <= 524 then -- Shandas
         Ms = "Shanda [Lv. 475]"
         QuestName = "SkyExp1Quest"
         LevelQuest = 2
         NameMon = "Shandas"
         CFrameQuest = CFrame.new(-7863.63672, 5545.49316, -379.826324, 0.362120807, -1.98046344e-08, -0.93213129, 4.05822291e-08, 1, -5.48095125e-09, 0.93213129, -3.58431969e-08, 0.362120807)
         CFrameMon = CFrame.new(-7685.12354, 5601.05127, -443.171509, 0.150056243, 1.79768236e-08, -0.988677442, 6.67798661e-09, 1, 1.91962481e-08, 0.988677442, -9.48289181e-09, 0.150056243)
      elseif MyLevel == 525 or MyLevel <= 549 then -- Royal Squad
         Ms = "Royal Squad [Lv. 525]"
         QuestName = "SkyExp2Quest"
         LevelQuest = 1
         NameMon = "Royal Squad"
         CFrameQuest = CFrame.new(-7902.66895, 5635.96387, -1411.71802, 0.0504222959, 2.5710392e-08, 0.998727977, 1.12541557e-07, 1, -3.14249675e-08, -0.998727977, 1.13982921e-07, 0.0504222959)
         CFrameMon = CFrame.new(-7685.02051, 5606.87842, -1442.729, 0.561947823, 7.69527464e-09, -0.827172697, -4.24974544e-09, 1, 6.41599973e-09, 0.827172697, -9.01838604e-11, 0.561947823)
      elseif MyLevel == 550 or MyLevel <= 624 then -- Royal Soldier
         Ms = "Royal Soldier [Lv. 550]"
         QuestName = "SkyExp2Quest"
         LevelQuest = 2
         NameMon = "Royal Soldier"
         CFrameQuest = CFrame.new(-7902.66895, 5635.96387, -1411.71802, 0.0504222959, 2.5710392e-08, 0.998727977, 1.12541557e-07, 1, -3.14249675e-08, -0.998727977, 1.13982921e-07, 0.0504222959)
         CFrameMon = CFrame.new(-7864.44775, 5661.94092, -1708.22351, 0.998389959, 2.28686137e-09, -0.0567218624, 1.99431383e-09, 1, 7.54200258e-08, 0.0567218624, -7.54117195e-08, 0.998389959)
      elseif MyLevel == 625 or MyLevel <= 649 then -- Galley Pirate
         Ms = "Galley Pirate [Lv. 625]"
         QuestName = "FountainQuest"
         LevelQuest = 1
         NameMon = "Galley Pirate"
         CFrameQuest = CFrame.new(5254.60156, 38.5011406, 4049.69678, -0.0504891425, -3.62066501e-08, -0.998724639, -9.87921389e-09, 1, -3.57534553e-08, 0.998724639, 8.06145284e-09, -0.0504891425)
         CFrameMon = CFrame.new(5595.06982, 41.5013695, 3961.47095, -0.992138803, -2.11610267e-08, -0.125142589, -1.34249509e-08, 1, -6.26613996e-08, 0.125142589, -6.04887518e-08, -0.992138803)
      elseif MyLevel >= 650 then -- Galley Captain
         Ms = "Galley Captain [Lv. 650]"
         QuestName = "FountainQuest"
         LevelQuest = 2
         NameMon = "Galley Captain"
         CFrameQuest = CFrame.new(5254.60156, 38.5011406, 4049.69678, -0.0504891425, -3.62066501e-08, -0.998724639, -9.87921389e-09, 1, -3.57534553e-08, 0.998724639, 8.06145284e-09, -0.0504891425)
         CFrameMon = CFrame.new(5658.5752, 38.5361786, 4928.93506, -0.996873081, 2.12391046e-06, -0.0790185928, 2.16989656e-06, 1, -4.96097414e-07, 0.0790185928, -6.66008248e-07, -0.996873081)
      end
   end
   if Sea2 then
      if MyLevel == 700 or MyLevel <= 724 then -- Raider [Lv. 700]
         Ms = "Raider [Lv. 700]"
         QuestName = "Area1Quest"
         LevelQuest = 1
         NameMon = "Raider"
         CFrameQuest = CFrame.new(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
         CFrameMon = CFrame.new(-737.026123, 39.1748352, 2392.57959, 0.272128761, 0, -0.962260842, -0, 1, -0, 0.962260842, 0, 0.272128761)
      elseif MyLevel == 725 or MyLevel <= 774 then -- Mercenary [Lv. 725]
         Ms = "Mercenary [Lv. 725]"
         QuestName = "Area1Quest"
         LevelQuest = 2
         NameMon = "Mercenary"
         CFrameQuest = CFrame.new(-424.080078, 73.0055847, 1836.91589, 0.253544956, -1.42165932e-08, 0.967323601, -6.00147771e-08, 1, 3.04272909e-08, -0.967323601, -6.5768397e-08, 0.253544956)
         CFrameMon = CFrame.new(-973.731995, 95.8733215, 1836.46936, 0.999135971, 2.02326991e-08, -0.0415605344, -1.90767793e-08, 1, 2.82094952e-08, 0.0415605344, -2.73922804e-08, 0.999135971)
      elseif MyLevel == 775 or MyLevel <= 799 then -- Swan Pirate [Lv. 775]
         Ms = "Swan Pirate [Lv. 775]"
         QuestName = "Area2Quest"
         LevelQuest = 1
         NameMon = "Swan Pirate"
         CFrameQuest = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
         CFrameMon = CFrame.new(970.369446, 142.653198, 1217.3667, 0.162079468, -4.85452638e-08, -0.986777723, 1.03357589e-08, 1, -4.74980872e-08, 0.986777723, -2.50063148e-09, 0.162079468)
      elseif MyLevel == 800 or MyLevel <= 874 then -- Factory Staff [Lv. 800]
         Ms = "Factory Staff [Lv. 800]"
         QuestName = "Area2Quest"
         LevelQuest = 2
         NameMon = "Factory Staff"
         CFrameQuest = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
         CFrameMon = CFrame.new(296.786499, 72.9948196, -57.1298141, -0.876037002, -5.32364979e-08, 0.482243896, -3.87658332e-08, 1, 3.99718729e-08, -0.482243896, 1.63222538e-08, -0.876037002)
      elseif MyLevel == 875 or MyLevel <= 899 then -- Marine Lieutenant [Lv. 875]
         Ms = "Marine Lieutenant [Lv. 875]"
         QuestName = "MarineQuest3"
         LevelQuest = 1
         NameMon = "Marine Lieutenant"
         CFrameQuest = CFrame.new(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
         CFrameMon = CFrame.new(-2913.26367, 73.0011826, -2971.64282, 0.910507619, 0, 0.413492233, 0, 1.00000012, 0, -0.413492233, 0, 0.910507619)
      elseif MyLevel == 900 or MyLevel <= 949 then -- Marine Captain [Lv. 900]
         Ms = "Marine Captain [Lv. 900]"
         QuestName = "MarineQuest3"
         LevelQuest = 2
         NameMon = "Marine Captain"
         CFrameQuest = CFrame.new(-2442.65015, 73.0511475, -3219.11523, -0.873540044, 4.2329841e-08, -0.486752301, 5.64383384e-08, 1, -1.43220786e-08, 0.486752301, -3.99823996e-08, -0.873540044)
         CFrameMon = CFrame.new(-1868.67688, 73.0011826, -3321.66333, -0.971402287, 1.06502087e-08, 0.237439692, 3.68856199e-08, 1, 1.06050372e-07, -0.237439692, 1.11775684e-07, -0.971402287)
      elseif MyLevel == 950 or MyLevel <= 974 then -- Zombie [Lv. 950]
         Ms = "Zombie [Lv. 950]"
         QuestName = "ZombieQuest"
         LevelQuest = 1
         NameMon = "Zombie"
         CFrameQuest = CFrame.new(-5492.79395, 48.5151672, -793.710571, 0.321800292, -6.24695815e-08, 0.946807742, 4.05616092e-08, 1, 5.21931227e-08, -0.946807742, 2.16082796e-08, 0.321800292)
         CFrameMon = CFrame.new(-5634.83838, 126.067039, -697.665039, -0.992770672, 6.77618939e-09, 0.120025545, 1.65461245e-08, 1, 8.04023372e-08, -0.120025545, 8.18070234e-08, -0.992770672)
      elseif MyLevel == 975 or MyLevel <= 999 then -- Vampire [Lv. 975]
         Ms = "Vampire [Lv. 975]"
         QuestName = "ZombieQuest"
         LevelQuest = 2
         NameMon = "Vampire"
         CFrameQuest = CFrame.new(-5492.79395, 48.5151672, -793.710571, 0.321800292, -6.24695815e-08, 0.946807742, 4.05616092e-08, 1, 5.21931227e-08, -0.946807742, 2.16082796e-08, 0.321800292)
         CFrameMon = CFrame.new(-6030.32031, 6.4377408, -1313.5564, -0.856965423, 3.9138893e-08, -0.515373945, -1.12178942e-08, 1, 9.45958547e-08, 0.515373945, 8.68467822e-08, -0.856965423)
      elseif MyLevel == 1000 or MyLevel <= 1049 then -- Snow Trooper [Lv. 1000] **
         Ms = "Snow Trooper [Lv. 1000]"
         QuestName = "SnowMountainQuest"
         LevelQuest = 1
         NameMon = "Snow Trooper"
         CFrameQuest = CFrame.new(604.964966, 401.457062, -5371.69287, 0.353063971, 1.89520435e-08, -0.935599446, -5.81846002e-08, 1, -1.70033754e-09, 0.935599446, 5.50377841e-08, 0.353063971)
         CFrameMon = CFrame.new(535.893433, 401.457062, -5329.6958, -0.999524176, 0, 0.0308452044, 0, 1, -0, -0.0308452044, 0, -0.999524176)
      elseif MyLevel == 1050 or MyLevel <= 1099 then -- Winter Warrior [Lv. 1050]
         Ms = "Winter Warrior [Lv. 1050]"
         QuestName = "SnowMountainQuest"
         LevelQuest = 2
         NameMon = "Winter Warrior"
         CFrameQuest = CFrame.new(604.964966, 401.457062, -5371.69287, 0.353063971, 1.89520435e-08, -0.935599446, -5.81846002e-08, 1, -1.70033754e-09, 0.935599446, 5.50377841e-08, 0.353063971)
         CFrameMon = CFrame.new(1223.7417, 454.575226, -5170.02148, 0.473996818, 2.56845354e-08, 0.880526543, -5.62456428e-08, 1, 1.10811016e-09, -0.880526543, -5.00510211e-08, 0.473996818)
      elseif MyLevel == 1100 or MyLevel <= 1124 then -- Lab Subordinate [Lv. 1100]
         Ms = "Lab Subordinate [Lv. 1100]"
         QuestName = "IceSideQuest"
         LevelQuest = 1
         NameMon = "Lab Subordinate"
         CFrameQuest = CFrame.new(-6060.10693, 15.9868021, -4904.7876, -0.411000341, -5.06538868e-07, 0.91163528, 1.26306062e-07, 1, 6.12581289e-07, -0.91163528, 3.66916197e-07, -0.411000341)
         CFrameMon = CFrame.new(-5769.2041, 37.9288292, -4468.38721, -0.569419742, -2.49055017e-08, 0.822046936, -6.96206541e-08, 1, -1.79282633e-08, -0.822046936, -6.74401548e-08, -0.569419742)
      elseif MyLevel == 1125 or MyLevel <= 1174 then -- Horned Warrior [Lv. 1125]
         Ms = "Horned Warrior [Lv. 1125]"
         QuestName = "IceSideQuest"
         LevelQuest = 2
         NameMon = "Horned Warrior"
         CFrameQuest = CFrame.new(-6060.10693, 15.9868021, -4904.7876, -0.411000341, -5.06538868e-07, 0.91163528, 1.26306062e-07, 1, 6.12581289e-07, -0.91163528, 3.66916197e-07, -0.411000341)
         CFrameMon = CFrame.new(-6400.85889, 24.7645149, -5818.63574, -0.964845479, 8.65926566e-08, -0.262817472, 3.98261392e-07, 1, -1.13260398e-06, 0.262817472, -1.19745812e-06, -0.964845479) --]]
      elseif MyLevel == 1175 or MyLevel <= 1199 then -- Magma Ninja [Lv. 1175]
         Ms = "Magma Ninja [Lv. 1175]"
         QuestName = "FireSideQuest"
         LevelQuest = 1
         NameMon = "Magma Ninja"
         CFrameQuest = CFrame.new(-5431.09473, 15.9868021, -5296.53223, 0.831796765, 1.15322464e-07, -0.555080295, -1.10814341e-07, 1, 4.17010995e-08, 0.555080295, 2.68240168e-08, 0.831796765)
         CFrameMon = CFrame.new(-5496.65576, 58.6890411, -5929.76855, -0.885073781, 0, -0.465450764, 0, 1.00000012, -0, 0.465450764, 0, -0.885073781)
      elseif MyLevel == 1200 or MyLevel <= 1249 then -- Lava Pirate [Lv. 1200]
         Ms = "Lava Pirate [Lv. 1200]"
         QuestName = "FireSideQuest"
         LevelQuest = 2
         NameMon = "Lava Pirate"
         CFrameQuest = CFrame.new(-5431.09473, 15.9868021, -5296.53223, 0.831796765, 1.15322464e-07, -0.555080295, -1.10814341e-07, 1, 4.17010995e-08, 0.555080295, 2.68240168e-08, 0.831796765)
         CFrameMon = CFrame.new(-5169.71729, 34.1234779, -4669.73633, -0.196780294, 0, 0.98044765, 0, 1.00000012, -0, -0.98044765, 0, -0.196780294)
      elseif MyLevel == 1250 or MyLevel <= 1274 then -- Ship Deckhand [Lv. 1250]
         Ms = "Ship Deckhand [Lv. 1250]"
         QuestName = "ShipQuest1"
         LevelQuest = 1
         NameMon = "Ship Deckhand"
         CFrameQuest = CFrame.new(1037.80127, 125.092171, 32911.6016, -0.244533166, -0, -0.969640911, -0, 1.00000012, -0, 0.96964103, 0, -0.244533136)
         CFrameMon = CFrame.new(1163.80872, 138.288452, 33058.4258, -0.998580813, 5.49076979e-08, -0.0532564968, 5.57436763e-08, 1, -1.42118655e-08, 0.0532564968, -1.71604082e-08, -0.998580813)
      elseif MyLevel == 1275 or MyLevel <= 1299 then -- Ship Engineer [Lv. 1275]
         Ms = "Ship Engineer [Lv. 1275]"
         QuestName = "ShipQuest1"
         LevelQuest = 2
         NameMon = "Ship Engineer"
         CFrameQuest = CFrame.new(1037.80127, 125.092171, 32911.6016, -0.244533166, -0, -0.969640911, -0, 1.00000012, -0, 0.96964103, 0, -0.244533136)
         CFrameMon = CFrame.new(916.666504, 44.0920448, 32917.207, -0.99746871, -4.85034697e-08, -0.0711069331, -4.8925461e-08, 1, 4.19294288e-09, 0.0711069331, 7.66126895e-09, -0.99746871)
      elseif MyLevel == 1300 or MyLevel <= 1324 then -- Ship Steward [Lv. 1300]
         Ms = "Ship Steward [Lv. 1300]"
         QuestName = "ShipQuest2"
         LevelQuest = 1
         NameMon = "Ship Steward"
         CFrameQuest = CFrame.new(968.80957, 125.092171, 33244.125, -0.869560242, 1.51905191e-08, -0.493826836, 1.44108379e-08, 1, 5.38534195e-09, 0.493826836, -2.43357912e-09, -0.869560242)
         CFrameMon = CFrame.new(918.743286, 129.591064, 33443.4609, -0.999792814, -1.7070947e-07, -0.020350717, -1.72559169e-07, 1, 8.91351277e-08, 0.020350717, 9.2628369e-08, -0.999792814)
      elseif MyLevel == 1325 or MyLevel <= 1349 then -- Ship Officer [Lv. 1325]
         Ms = "Ship Officer [Lv. 1325]"
         QuestName = "ShipQuest2"
         LevelQuest = 2
         NameMon = "Ship Officer"
         CFrameQuest = CFrame.new(968.80957, 125.092171, 33244.125, -0.869560242, 1.51905191e-08, -0.493826836, 1.44108379e-08, 1, 5.38534195e-09, 0.493826836, -2.43357912e-09, -0.869560242)
         CFrameMon = CFrame.new(786.051941, 181.474106, 33303.2969, 0.999285698, -5.32193063e-08, 0.0377905183, 5.68968588e-08, 1, -9.62386864e-08, -0.0377905183, 9.83201005e-08, 0.999285698)
      elseif MyLevel == 1350 or MyLevel <= 1374 then -- Arctic Warrior [Lv. 1350]
         Ms = "Arctic Warrior [Lv. 1350]"
         QuestName = "FrostQuest"
         LevelQuest = 1
         NameMon = "Arctic Warrior"
         CFrameQuest = CFrame.new(5669.43506, 28.2117786, -6482.60107, 0.888092756, 1.02705066e-07, 0.459664226, -6.20391774e-08, 1, -1.03572376e-07, -0.459664226, 6.34646895e-08, 0.888092756)
         CFrameMon = CFrame.new(5995.07471, 57.3188477, -6183.47314, 0.702747107, -1.53454167e-07, -0.711440146, -1.08168464e-07, 1, -3.22542007e-07, 0.711440146, 3.03620908e-07, 0.702747107)
      elseif MyLevel == 1375 or MyLevel <= 1424 then -- Snow Lurker [Lv. 1375]
         Ms = "Snow Lurker [Lv. 1375]"
         QuestName = "FrostQuest"
         LevelQuest = 2
         NameMon = "Snow Lurker"
         CFrameQuest = CFrame.new(5669.43506, 28.2117786, -6482.60107, 0.888092756, 1.02705066e-07, 0.459664226, -6.20391774e-08, 1, -1.03572376e-07, -0.459664226, 6.34646895e-08, 0.888092756)
         CFrameMon = CFrame.new(5518.00684, 60.5559731, -6828.80518, -0.650781393, -3.64292951e-08, 0.759265184, -4.07668654e-09, 1, 4.44854642e-08, -0.759265184, 2.58550248e-08, -0.650781393)
      elseif MyLevel == 1425 or MyLevel <= 1449 then -- Sea Soldier [Lv. 1425]
         Ms = "Sea Soldier [Lv. 1425]"
         QuestName = "ForgottenQuest"
         LevelQuest = 1
         NameMon = "Sea Soldier"
         CFrameQuest = CFrame.new(-3052.99097, 236.881363, -10148.1943, -0.997911751, 4.42321983e-08, 0.064591676, 4.90968759e-08, 1, 7.37270085e-08, -0.064591676, 7.67442998e-08, -0.997911751)
         CFrameMon = CFrame.new(-3029.78467, 66.944252, -9777.38184, -0.998552859, 1.09555076e-08, 0.0537791774, 7.79564235e-09, 1, -5.89660658e-08, -0.0537791774, -5.84614881e-08, -0.998552859)
      elseif MyLevel >= 1450 then -- Water Fighter [Lv. 1450]
         Ms = "Water Fighter [Lv. 1450]"
         QuestName = "ForgottenQuest"
         LevelQuest = 2
         NameMon = "Water Fighter"
         CFrameQuest = CFrame.new(-3052.99097, 236.881363, -10148.1943, -0.997911751, 4.42321983e-08, 0.064591676, 4.90968759e-08, 1, 7.37270085e-08, -0.064591676, 7.67442998e-08, -0.997911751)
         CFrameMon = CFrame.new(-3262.00098, 298.699615, -10553.6943, -0.233570755, -4.57538185e-08, 0.972339869, -5.80986068e-08, 1, 3.30992194e-08, -0.972339869, -4.87605725e-08, -0.233570755)
      end
   end
   if ThreeWorld then
      if MyLevel == 1500 or MyLevel <= 1524 or SeletMon == "Pirate Millionaire [MyLevel. 1500]" then -- Pirate Millionaire
         Ms = "Pirate Millionaire [Lv. 1500]"
         NameMon = "Pirate Millionaire"
         QuestName = "PiratePortQuest"
         LevelQuest = 1
         Reward = "Reward:\n$13,000\n35,000,000 Exp."
         CFrameQ = CFrame.new(-289.61752319336, 43.819011688232, 5580.0903320313)
         CFrameMon = CFrame.new(-435.68109130859, 189.69866943359, 5551.0756835938)
      elseif MyLevel == 1525 or MyLevel <= 1574 or SeletMon == "Pistol Billionaire [Lv. 1525]" then -- Pistol Billoonaire
         Ms = "Pistol Billionaire [Lv. 1525]"
         NameMon = "Pistol Billionaire"
         QuestName = "PiratePortQuest"
         LevelQuest = 2
         Reward = "Reward:\n$15,000\n37,500,000 Exp."
         CFrameQ = CFrame.new(-289.61752319336, 43.819011688232, 5580.0903320313)
         CFrameMon = CFrame.new(-236.53652954102, 217.46676635742, 6006.0883789063)
      elseif MyLevel == 1575 or MyLevel <= 1599 or SeletMon == "Dragon Crew Warrior [Lv. 1575]" then -- Dragon Crew Warrior
         Ms = "Dragon Crew Warrior [Lv. 1575]"
         NameMon = "Amazon Quest Giver"
         QuestName = "AmazonQuest"
         LevelQuest = 1
         Reward = "Reward:\n$13,000\n40,000,000 Exp."
         CFrameQuest = CFrame.new(5833.1147460938, 51.60498046875, -1103.0693359375)
         CFrameMon = CFrame.new(6301.9975585938, 104.77153015137, -1082.6075439453)
      elseif MyLevel == 1600 or MyLevel <= 1624 or SeletMon == "Dragon Crew Archer [Lv. 1600]" then -- Dragon Crew Archer
         Ms = "Dragon Crew Archer [Lv. 1600]"
         NameMon = "Dragon Crew Archer"
         QuestName = "AmazonQuest"
         LevelQuest = 2
         Reward = "Reward:\n$15,000\n42,500,000 Exp."
         CFrameQuest = CFrame.new(5833.1147460938, 51.60498046875, -1103.0693359375)
         CFrameMon = CFrame.new(6831.1171875, 441.76708984375, 446.58615112305)
      elseif MyLevel == 1625 or MyLevel <= 1649 or SeletMon == "Female Islander [Lv. 1625]" then -- Female Islander
         Ms = "Female Islander [Lv. 1625]"
         NameMon = "Female Islander"
         QuestName = "AmazonQuest2"
         LevelQuest = 1
         Reward = "Reward:\n$13,000\n45,500,000 Exp."
         CFrameQuest = CFrame.new(5446.8793945313, 601.62945556641, 749.45672607422)
         CFrameMon = CFrame.new(5792.5166015625, 848.14392089844, 1084.1818847656)
      elseif MyLevel == 1650 or MyLevel <= 1699 or SeletMon == "Giant Islander [Lv. 1650]" then -- Giant Islander
         Ms = "Giant Islander [Lv. 1650]"
         NameMon = "Giant"
         QuestName = "AmazonQuest2"
         LevelQuest = 2
         Reward = "Reward:\n$15,000\n48,000,000 Exp."
         CFrameQuest = CFrame.new(5446.8793945313, 601.62945556641, 749.45672607422)
         CFrameMon = CFrame.new(5009.5068359375, 664.11071777344, -40.960144042969)
      elseif MyLevel == 1700 or MyLevel <= 1724 or SeletMon == "Marine Commodore [Lv. 1700]" then -- Marine Commodore
         Ms = "Marine Commodore [Lv. 1700]"
         NameMon = "Marine Commodore"
         QuestName = "MarineTreeIsland"
         LevelQuest = 1
         Reward = "Reward:\n$13,000\n51,000,000 Exp."
         CFrameQuest = CFrame.new(2179.98828125, 28.731239318848, -6740.0551757813)
         CFrameMon = CFrame.new(2198.0063476563, 128.71075439453, -7109.5043945313)
      elseif MyLevel == 1725 or MyLevel <= 1774 or SeletMon == "Marine Rear Admiral [Lv. 1725]" then -- Marine Rear Admiral
         Ms = "Marine Rear Admiral [Lv. 1725]"
         NameMon = "Marine Rear Admiral"
         QuestName = "MarineTreeIsland"
         LevelQuest = 2
         Reward = "Reward:\n$15,000\n53,500,000 Exp."
         CFrameQuest = CFrame.new(2179.98828125, 28.731239318848, -6740.0551757813)
         CFrameMon = CFrame.new(3294.3142089844, 385.41125488281, -7048.6342773438)
      elseif MyLevel == 1775 or MyLevel <= 1799 or SeletMon == "Fishman Raider [Lv. 1775]" then -- Fishman Raide
         Ms = "Fishman Raider [Lv. 1775]"
         NameMon = "Fishman Raider"
         QuestName = "DeepForestIsland3"
         LevelQuest = 1
         Reward = "Reward:\n$13,000\n56,000,000 Exp."
         CFrameQuest = CFrame.new(-10582.759765625, 331.78845214844, -8757.666015625)
         CFrameMon = CFrame.new(-10553.268554688, 521.38439941406, -8176.9458007813)
      elseif MyLevel == 1800 or MyLevel <= 1824 or SeletMon == "Fishman Captain [Lv. 1800]" then -- Fishman Captain
         Ms = "Fishman Captain [Lv. 1800]"
         NameMon = "Fishman Captain"
         QuestName = "DeepForestIsland3"
         LevelQuest = 2
         Reward = "Reward:\n$15,000\n58,500,000 Exp."
         CFrameQuest = CFrame.new(-10583.099609375, 331.78845214844, -8759.4638671875)
         CFrameMon = CFrame.new(-10789.401367188, 427.18637084961, -9131.4423828125)
      elseif MyLevel == 1825 or MyLevel <= 1849 or SeletMon == "Forest Pirate [Lv. 1825]" then -- Forest Pirate
         Ms = "Forest Pirate [Lv. 1825]"
         NameMon = "Forest Pirate"
         QuestName = "DeepForestIsland"
         LevelQuest = 1
         Reward = "Reward:\n$13,000\n61,000,000 Exp."
         CFrameQuest = CFrame.new(-13232.662109375, 332.40396118164, -7626.4819335938)
         CFrameMon = CFrame.new(-13489.397460938, 400.30349731445, -7770.251953125)
      elseif MyLevel == 1850 or MyLevel <= 1899 or SeletMon == "Mythological Pirate [Lv. 1850]" then -- Mythological Pirate
         Ms = "Mythological Pirate [Lv. 1850]"
         NameMon = "Mythological Pirate"
         QuestName = "DeepForestIsland"
         LevelQuest = 2
         Reward = "Reward:\n$13,000\n64,000,000 Exp."
         CFrameQuest = CFrame.new(-13232.662109375, 332.40396118164, -7626.4819335938)
         CFrameMon = CFrame.new(-13508.616210938, 582.46228027344, -6985.3037109375)
      elseif MyLevel == 1900 or MyLevel <= 1924 or SeletMon == "Jungle Pirate [Lv. 1900]" then -- Jungle Pirate
         Ms = "Jungle Pirate [Lv. 1900]"
         NameMon = "Jungle Pirate"
         QuestName = "DeepForestIsland2"
         LevelQuest = 1
         Reward = "Reward:\n$13,000\n67,000,000 Exp."
         CFrameQuest = CFrame.new(-12682.096679688, 390.88653564453, -9902.1240234375)
         CFrameMon = CFrame.new(-12267.103515625, 459.75262451172, -10277.200195313)
      elseif MyLevel == 1925 or MyLevel <= 1974 or SeletMon == "Musketeer Pirate [Lv. 1925]" then -- Musketeer Pirate
         Ms = "Musketeer Pirate [Lv. 1925]"
         NameMon = "Musketeer Pirate"
         QuestName = "DeepForestIsland2"
         LevelQuest = 2
         Reward = "Reward:\n$15,000\n70,000,000 Exp."
         CFrameQuest = CFrame.new(-12682.096679688, 390.88653564453, -9902.1240234375)
         CFrameMon = CFrame.new(-13291.5078125, 520.47338867188, -9904.638671875)
      elseif MyLevel == 1975 or MyLevel <= 1999 then
         Ms = "Reborn Skeleton [Lv. 1975]"
         NameMon = "Reborn Skeleton"
         QuestName = "HauntedQuest1"
         LevelQuest = 1
         Reward = "Reward:\n$13,000\n73,000,000 Exp."
         CFrameQuest = CFrame.new(-9480.80762, 142.130661, 5566.37305, -0.00655503059, 4.52954225e-08, -0.999978542, 2.04920472e-08, 1, 4.51620679e-08, 0.999978542, -2.01955679e-08, -0.00655503059)
         CFrameMon = CFrame.new(-8761.77148, 183.431747, 6168.33301, 0.978073597, -1.3950732e-05, -0.208259016, -1.08073925e-06, 1, -7.20630269e-05, 0.208259016, 7.07080399e-05, 0.978073597)
      elseif MyLevel == 2000 or MyLevel <= 2024 then
         Ms = "Living Zombie [Lv. 2000]"
         NameMon = "Living Zombie"
         QuestName = "HauntedQuest1"
         LevelQuest = 2
         Reward = "Reward:\n$13,250\n75,500,000 Exp."
         CFrameQuest = CFrame.new(-9480.80762, 142.130661, 5566.37305, -0.00655503059, 4.52954225e-08, -0.999978542, 2.04920472e-08, 1, 4.51620679e-08, 0.999978542, -2.01955679e-08, -0.00655503059)
         CFrameMon = CFrame.new(-10103.7529, 238.565979, 6179.75977, 0.999474227, 2.77547141e-08, 0.0324240364, -2.58006327e-08, 1, -6.06848474e-08, -0.0324240364, 5.98163865e-08, 0.999474227)
      elseif MyLevel == 2025 or MyLevel <= 2049 then
         Ms = "Demonic Soul [Lv. 2025]"
         NameMon = "Demonic Soul"
         QuestName = "HauntedQuest2"
         LevelQuest = 1
         Reward = "Reward:\n$13,500\n78,000,000 Exp."
         CFrameQuest = CFrame.new(-9515.39551, 172.266037, 6078.89746, 0.0121199936, -9.78649624e-08, 0.999926567, 2.30358754e-08, 1, 9.75929382e-08, -0.999926567, 2.18513581e-08, 0.0121199936)
         CFrameMon = CFrame.new(-9709.30762, 204.695892, 6044.04688, -0.845798075, -3.4587876e-07, -0.533503294, -4.46235369e-08, 1, -5.77571257e-07, 0.533503294, -4.64701827e-07, -0.845798075)
      elseif MyLevel >= 2050 then
         Ms = "Posessed Mummy [Lv. 2050]"
         NameMon = "Posessed Mummy"
         QuestName = "HauntedQuest2"
         LevelQuest = 2
         Reward = "Reward:\n$13,750\n80,500,000 Exp."
         CFrameQuest = CFrame.new(-9515.39551, 172.266037, 6078.89746, 0.0121199936, -9.78649624e-08, 0.999926567, 2.30358754e-08, 1, 9.75929382e-08, -0.999926567, 2.18513581e-08, 0.0121199936)
         CFrameMon = CFrame.new(-9554.11035, 65.6141663, 6041.73584, -0.877069294, 5.33355795e-08, -0.480364174, 2.06420765e-08, 1, 7.33423562e-08, 0.480364174, 5.44105987e-08, -0.877069294)
      end
   end
end
game:GetService("RunService").Heartbeat:Connect(function()
    pcall(function()
        CheckQuest()
   if not game.Workspace:FindFirstChild(NameMon) then
    local part = Instance.new("Part")
    part.Name = NameMon
    part.Position = Vector3.new(0, 10, 0)
    part.Anchored = true
    part.CFrame = CFrameQuest
    part.Transparency = 1
    part.Parent = game.Workspace
 end
end)
end)


local player = game.Players.LocalPlayer
local TeleportService = game:GetService("TeleportService")
local level1Id = 7899144215

local DinoPage = powerx:addPage("AutoFarm", 7040391851)
local Home = DinoPage:addSection("AutoFarm ")


function itemequip(namex)
   pcall(function()
   local ToolSe = tostring(namex)
   local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
   game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
   end)
end

function tweenteleport(Speed,Part)
   local Distancex = (Vector3.new(Part) - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
   local Speexd = Speed -- ความเร็วของมึง
   tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
   tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(Part)})
   tweenx:Play()
   wait(Distancex/Speexd)
end
local magnitude = 0
game:GetService("RunService").Heartbeat:Connect(function()
    pcall(function()
    CheckQuest()
    magnitude = (workspace[NameMon].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
    end)
end)
Home:addToggle("Auto Farm",nil,function(value)
_G.AutoFarm = value
while _G.AutoFarm do game:GetService("RunService").Heartbeat:wait()
   pcall(function()
    CheckQuest()
   magnitude = (workspace[NameMon].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
   if magnitude < 2250 then
      if _G.AutoFarm == true then
         if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
            if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
               if string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
                  for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                     if v.Name == Ms then
                        if v.Humanoid.Health > 0 then
                           repeat game:GetService("RunService").Heartbeat:wait()
                              click()
                              itemequip(weapongg)
                              v.Humanoid:ChangeState(11)
                              MinHealth = v.Humanoid.MaxHealth * 35 / 100
                              local magnitudX = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
                              if v.Humanoid.Health > MinHealth then
                                 local Distance = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
                                 local Speed = 1250 -- ความเร็วของมึง
                                 tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
                                 tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,0,13)})
                                 tween:Play()
                              else
                                 tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(0.5, Enum.EasingStyle.Linear)
                                 tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,14,0)})
                                 tween:Play()
                              end
                              game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
                              game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
                           until v.Humanoid.Health <= 0 or _G.AutoFarm == false
                        elseif v.Humanoid.Health <= 0  then
                           local Distance = (Vector3.new(CFrameMon) - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
                           local Speed = 10000 -- ความเร็วของมึง
                           tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
                           tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrameMon})
                           tween:Play()
                           wait(Distance/Speed)
                        end
                     end
                  end
               else
                  CheckQuest()
                  local args = {
                     [1] = "AbandonQuest"
                  }

                  game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))

                  game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
               end
            elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
               if _G.AutoFarm == true then
                  CheckQuest()
                  local Distance = (game.Workspace[NameMon].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
                  local Speed = 500 -- ความเร็วของมึง
                  tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
                  tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrameQuest})
                  tween:Play()
                  print(magnitude)
                  wait(Distance/Speed)
                  wait(3)

                  local args = {
                     [1] = "StartQuest",
                     [2] = QuestName,
                     [3] = LevelQuest
                  }

                  game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
               end
            end
         else
            CheckQuest()
            local Distance = (game.Workspace[NameMon].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
            local Speed = 1500 -- ความเร็วของมึง
            tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear)
            tween = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrameMon})
            print(magnitude)
            tween:Play()
            wait(Distance/Speed)
         end
      end
   else
      CheckQuest()
      local Distancex = (game.Workspace[NameMon].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
      local Speexd = 99 -- ความเร็วของมึง
      tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
      tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrameQuest})
      tweenx:Play()
      print(magnitude)
      print(Distancex/Speexd)
      wait(Distancex/Speexd)
      wait(3)
      local args = {
         [1] = "StartQuest",
         [2] = QuestName,
         [3] = LevelQuest
      }

      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   end
   end)
end
end)

function fruitinbackpack()
   for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
      if v.ClassName == "Tool" then
         if v.ToolTip == "Blox Fruit" then
            fruitname = v.Name
         end
      end
   end
   return fruitname
end

function fruitinbackpack2()
   for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
      if v.ClassName == "Tool" then
         if v.ToolTip == "Blox Fruit" then
            xxd = v.Name
         end
      end
   end
   return xxd
end

function gunname()
   for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
      if v.ClassName == "Tool" then
         if v.ToolTip == "Gun" then
            xxd = v.Name
         end
      end
   end
   return xxd
end

function equipfruit()
   if game.Players.LocalPlayer.Backpack:FindFirstChild(fruitinbackpack2()) then
      local ToolSe = tostring(fruitinbackpack2())
      local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
      game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
   end
end

function equipcombat(a)
   if game.Players.LocalPlayer.Backpack:FindFirstChild(a) then
      local ToolSe = tostring(a)
      local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
      game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
   end
end
function itemequip(namex)
    pcall(function()
    local ToolSe = tostring(namex)
    local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
    game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
    end)
 end
 Home:addButton("Redeem All Code", function()

   local string_1 = "UPD14";
   local Target = game:GetService("ReplicatedStorage").Remotes.Redeem;
   Target:InvokeServer(string_1);
   
   local string_1 = "Sub2NoobMaster123";
   local Target = game:GetService("ReplicatedStorage").Remotes.Redeem;
   Target:InvokeServer(string_1);
   
   local string_1 = "Sub2Daigrock";
   local Target = game:GetService("ReplicatedStorage").Remotes.Redeem;
   Target:InvokeServer(string_1);
   
   local string_1 = "Axiore";
   local Target = game:GetService("ReplicatedStorage").Remotes.Redeem;
   Target:InvokeServer(string_1);
   
   local string_1 = "TantaiGaming";
   local Target = game:GetService("ReplicatedStorage").Remotes.Redeem;
   Target:InvokeServer(string_1);
   
   local string_1 = "StrawHatMaine";
   local Target = game:GetService("ReplicatedStorage").Remotes.Redeem;
   Target:InvokeServer(string_1);
   
   local string_1 = "Sub2OfficialNoobie";
   local Target = game:GetService("ReplicatedStorage").Remotes.Redeem;
   Target:InvokeServer(string_1);
   
   local string_1 = "TheGreatAce";
   local Target = game:GetService("ReplicatedStorage").Remotes.Redeem;
   Target:InvokeServer(string_1);
   
   local string_1 = "Fudd10";
   local Target = game:GetService("ReplicatedStorage").Remotes.Redeem;
   Target:InvokeServer(string_1);
   
   local string_1 = "Bignews";
   local Target = game:GetService("ReplicatedStorage").Remotes.Redeem;
   Target:InvokeServer(string_1);
   
   local string_1 = "UPD15";
   local Target = game:GetService("ReplicatedStorage").Remotes.Redeem;
   Target:InvokeServer(string_1);
   
end)
Home:addToggle("Fast Attack",nil,function(value)
_G.FastAttack = value
end)
Home:addToggle("Bring Mob",nil,function(value)
_G.bringmob = value
end)

ToolName = {}
for i, v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
   if v:IsA("Tool") then
      table.insert(ToolName, v.Name)
   end
end
for i, v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
   if v:IsA("Tool") then
      table.insert(ToolName, v.Name)
   end
end
Home:addDropdown("Select Weapon", ToolName, function(list)
   weapongg = list
end)

Home:addButton("Refresh Weapon", function()
table.clear(ToolName)
for i, v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
   if v:IsA("Tool") then
      table.insert(ToolName, v.Name)
   end
end
for i, v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
   if v:IsA("Tool") then
      table.insert(ToolName, v.Name)
   end
end
end)

Home:addToggle("Invisble Mob",nil,function(value)
   _G.inv = value
   while _G.inv do wait()
      pcall(function()
      for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
         if v.ClassName == "MeshPart" then
            v.Transparency = 1
         end
      end
      for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
         if v.Name == "Head" then
            v.Transparency = 1
         end
      end
      for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
         if v.ClassName == "Accessory" then
            v.Handle.Transparency = 1
         end
      end
      for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
         if v.ClassName == "Decal" then
            v.Transparency = 1
         end
      end
      end)
   end
end)

Home:addToggle("Auto Farm Mastery Fruit",nil,function(value)
_G.AutoFarmMas = value
while _G.AutoFarmMas do wait()
   pcall(function()
   if _G.AutoFarmMas == true then
      itemequip(weapongg)
      CheckQuest()
      if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
         if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
            if string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
               for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                  if v.Name == Ms then
                     if v.Humanoid.Health > 0 then
                        repeat wait()
                           click()
                           if OldWorld then
                              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
                           elseif Sea2 then
                              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,0)
                           elseif ThreeWorld then
                              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,0,15)
                           end
                           itemequip(weapongg)
                           v.HumanoidRootPart.Size = Vector3.new(30,30,30)
                           v.HumanoidRootPart.Transparency = 0.99
                           v.HumanoidRootPart.CanCollide = true
                           v.Humanoid:ChangeState(11)
                           game.Players.LocalPlayer.Character.HumanoidRootPart.CanCollide = false
                           v.Humanoid.WalkSpeed = 0
                           game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
                           MinHealth = v.Humanoid.MaxHealth * 15 / 100
                           if v.Humanoid.Health < MinHealth then
                              equipfruit()
                              local args = {
                                 [1] = "Z",
                                 [2] = v.HumanoidRootPart.Position
                              }

                              game:GetService("Players").LocalPlayer.Character:FindFirstChild(fruitinbackpack()).RemoteFunction:InvokeServer(unpack(args))
                              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,0,15)
                              game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
                              local args = {
                                 [1] = "X",
                                 [2] = v.HumanoidRootPart.Position
                              }

                              game:GetService("Players").LocalPlayer.Character:FindFirstChild(fruitinbackpack()).RemoteFunction:InvokeServer(unpack(args))
                              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,0,15)
                              game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
                              local args = {
                                 [1] = "C",
                                 [2] = v.HumanoidRootPart.Position
                              }

                              game:GetService("Players").LocalPlayer.Character:FindFirstChild(fruitinbackpack()).RemoteFunction:InvokeServer(unpack(args))
                              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,0,15)
                              game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
                              local args = {
                                 [1] = "V",
                                 [2] = v.HumanoidRootPart.Position
                              }

                              game:GetService("Players").LocalPlayer.Character:FindFirstChild(fruitinbackpack()).RemoteFunction:InvokeServer(unpack(args))
                              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,0,15)
                              game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
                           end
                           itemequip(weapongg)
                        until v.Humanoid.Health <= 0 or _G.AutoFarmMas == false
                     elseif v.Humanoid.Health <= 1 then
                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon

                     end
                  end
               end
            else
               CheckQuest()

               local args = {
                  [1] = "AbandonQuest"
               }

               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))

               game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
            end
         elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
            if _G.AutoFarmMas == true then
               CheckQuest()
               game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameQuest
               wait(1)
               local args = {
                  [1] = "StartQuest",
                  [2] = NaemQuest,
                  [3] = LevelQuest
               }

               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
         end
      else
         CheckQuest()
         game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
      end
   end
   end)
end
end)
Home:addToggle("Auto Farm Mastery Gun",nil,function(value)
_G.AutoFarmMasGun = value
while _G.AutoFarmMasGun do wait()
   pcall(function()
   equipgun()
   if _G.AutoFarmMasGun == true then
      CheckQuest()
      if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
         if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
            if string.find(game.Players.LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
               for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                  if v.Name == Ms then
                     local magnitude = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
                     if magnitude < 1000 then
                        if v.Humanoid.Health > 0 then
                           repeat wait()
                              equipgun()
                              itemequip(weapongg)
                              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,25,0)
                              v.HumanoidRootPart.Size = Vector3.new(30,30,30)
                              v.HumanoidRootPart.Transparency = 0.99
                              v.HumanoidRootPart.CanCollide = true
                              v.Humanoid:ChangeState(11)
                              game.Players.LocalPlayer.Character.HumanoidRootPart.CanCollide = false
                              v.Humanoid.WalkSpeed = 0
                              game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
                              local args = {
                                 [1] = v.Head.Position,
                                 [2] = workspace.Enemies:FindFirstChild(Ms).HumanoidRootPart
                              }
                              game:GetService("Players").LocalPlayer.Character[gunname()].RemoteFunctionShoot:InvokeServer(unpack(args))
                           until v.Humanoid.Health <= 0 or _G.AutoFarmMasGun == false
                           itemequip(weapongg)
                        elseif v.Humanoid.Health <= 1 then
                           game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
                        end
                     else
                        CheckQuest()
                        local Distancex = (game.Workspace[NameMon].Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
                        local Speexd = 100 -- ความเร็วของมึง
                        tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
                        tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game.Workspace[NameMon].CFrame})
                        tweenx:Play()
                        wait(Distancex/Speexd)
                     end
                  end
               end
            else
               CheckQuest()

               local args = {
                  [1] = "AbandonQuest"
               }

               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))

               game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
            end
         elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
            if _G.AutoFarmMasGun == true then
               CheckQuest()
               game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameQuest
               wait(4)
               local args = {
                  [1] = "StartQuest",
                  [2] = NaemQuest,
                  [3] = LevelQuest
               }

               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
         end
      else
         CheckQuest()
         game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrameMon
      end
   end
   end)
end
end)
function equipgun()
   pcall(function()
   for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
      if v.ClassName == "Tool" then
         if v.ToolTip == "Gun" then
            if game.Players.LocalPlayer.Backpack:FindFirstChild(v.Name) then
               local ToolSe = tostring(v.Name)
               local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
               game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
            end
         end
      end
   end
   end)
end
game:GetService("RunService").Heartbeat:Connect(function()
if _G.farmmasfruit then
   game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
end
end)
Home:addToggle("Auto Farm All Boss",nil,function(value)
_G.AutoFarmAllBoss = value
while _G.AutoFarmAllBoss do wait()
   pcall(function()
   itemequip(weapongg)
   for i,v in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
      if string.find(v.Name , "Boss") then
         repeat wait()
            local magnitude = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
            if magnitude < 1000 then
               itemequip(weapongg)
               game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,8)
               v.HumanoidRootPart.Size = Vector3.new(40,40,40)
               v.HumanoidRootPart.Transparency = 0.85
               v.HumanoidRootPart.CanCollide = true
               v.Humanoid.WalkSpeed = 0
               v.Humanoid:ChangeState(11)
               click()
            else
               local Distancex = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
               local Speexd = 90 -- ความเร็วของมึง
               tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
               tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = v.HumanoidRootPart.CFrame*CFrame.new(0,30,0)})
               tweenx:Play()
               wait(Distancex/Speexd)
            end
         until v.Humanoid.Health <= 0 or _G.AutoFarmAllBoss == false
      end
   end
   end)
end
end)

local LocalPlayer = game:GetService'Players'.LocalPlayer
local originalstam = LocalPlayer.Character.Energy.Value
function infinitestam()
   LocalPlayer.Character.Energy.Changed:connect(function()
   if InfinitsEnergy then
      LocalPlayer.Character.Energy.Value = originalstam
   end
   end)
end

local Main2 =  DinoPage:addSection("Menu Auto")

function tweenteleoirtxx(XXXXx,Arfggg)
   local Distance = (XXXXx - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
   local Speed = 149
   game:GetService("TweenService"):Create(
   game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart,
   TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear),
   {CFrame = Arfggg}
   ):Play()
   _G.NoClip = true
   wait(Distance/Speed)
   _G.NoClip = false
end

Main2:addToggle("Auto New World",nil,function(vu)
   _G.AutoNew = vu
end)
spawn(function()
   while wait(.1) do
      if _G.AutoNew then
         local MyLevel = game.Players.localPlayer.Data.Level.Value
         if MyLevel >= 200 and OldWorld then
            SelectToolWeapon = "Key"
            tweenteleoirtxx(Vector3.new(4849.29883, 5.65138149, 719.611877),CFrame.new(4849.29883, 5.65138149, 719.611877))

            wait(0.5)
            local args = {
               [1] = "DressrosaQuestProgress",
               [2] = "Detective"
            }
            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            wait(0.5)
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Key") then
               local tool = game.Players.LocalPlayer.Backpack:FindFirstChild("Key")
               wait(.4)
               game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
            end
            tweenteleoirtzz(Vector3.new(1347.7124, 37.3751602, -1325.6488),CFrame.new(1347.7124, 37.3751602, -1325.6488))
            wait(0.5)
            function click()
               require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1} 
               require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework).activeController.timeToNextAttack = 100
               game:GetService'VirtualUser':CaptureController()
               game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)  
               require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1} 
               game:GetService'VirtualUser':CaptureController()
               game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
               require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1} 
               game:GetService'VirtualUser':CaptureController()
               game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
            end
            if game.Workspace.Enemies:FindFirstChild("Ice Admiral [Lv. 700] [Boss]") and game.Workspace.Map.Ice.Door.CanCollide == false and game.Workspace.Map.Ice.Door.Transparency == 1 then
               CheckBoss = true
               SelectToolWeapon = SelectToolWeaponOld
               for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
                  if CheckBoss and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and v.Name == "Ice Admiral [Lv. 700] [Boss]" then
                     repeat wait(.1)
                        pcall(function() 
                           v.HumanoidRootPart.Transparency = 0.5
                           v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
                           v.HumanoidRootPart.BrickColor = BrickColor.new("White")
                           v.HumanoidRootPart.CanCollide = false
                           game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame*CFrame.new(0, 10, 10)
                           click()
                        end)
                     until not CheckBoss or not v.Parent or v.Humanoid.Health <= 0
                  end
               end
               CheckBoss = false
               wait(0.5)
               tweenteleoirtxx(Vector3.new(1166.23743, 7.65220165, 1728.36487),CFrame.new(1166.23743, 7.65220165, 1728.36487))
               wait(0.5)
               local args = {
                   [1] = "TravelDressrosa" -- OLD WORLD to NEW WORLD
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            else
               if game.Players.LocalPlayer.Backpack:FindFirstChild("Key") then
                  local tool = game.Players.LocalPlayer.Backpack:FindFirstChild("Key")
                  wait(.4)
                  game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
               end
               tweenteleoirtxx(Vector3.new(1347.7124, 37.3751602, -1325.6488),CFrame.new(1347.7124, 37.3751602, -1325.6488))
            end 
         end
      end 
   end
end)
Main2:addToggle("Auto Saber",nil,function(value)
   if value then
      local MyLevel = game.Players.localPlayer.Data.Level.Value
      if MyLevel == 200 or MyLevel <= 2100 then
         ply = game.Players.LocalPlayer.Character.HumanoidRootPart
         tweenteleoirtzz(Vector3.new(-1249.77222, 11.8870859, 341.356476),CFrame.new(-1249.77222, 11.8870859, 341.356476))
      
         ply.CFrame = CFrame.new(-1180.89563, 21.0007095, 187.861374, -0.866141438, -2.23321149e-05, -0.499799222, 2.23321149e-05, 1, -8.33832528e-05, 0.499799222, -8.33832528e-05, -0.866141438)
         wait(.5)
         ply.CFrame = CFrame.new(-1421.19995, 44.5000229, 21.6000061, -0.866039991, -0.499974549, -5.5283308e-06, -5.5283308e-06, 2.06232071e-05, -0.99999994, 0.499974549, -0.866040051, -2.06232071e-05)
         wait(.5)
         ply.CFrame = CFrame.new(-1648.49451, 19.5000286, 437.794678, -0.190788865, -0.981631041, 4.50909138e-05, 4.50909138e-05, -5.47170639e-05, -1, 0.981631041, -0.190788865, 5.47170639e-05)
         wait(.5)
         ply.CFrame = CFrame.new(-1324.10144, 31.4560413, -461.404114, 0.766120374, 2.95190748e-05, 0.642697096, 2.95190748e-05, 1, -8.11179052e-05, -0.642697096, 8.11179052e-05, 0.766120374)
         wait(.5)
         ply.CFrame = CFrame.new(-1611.09485, 16.2000656, 133.827881, 0.499959469, -0, -0.866048813, 0, 1, -0, 0.866048813, 0, 0.499959469)
         wait(.5)
         ply.CFrame = CFrame.new(-1154.34534, 2.45317268, -701.115295, 0.888653398, 6.63873134e-09, -0.45857957, -7.61690178e-09, 1, -2.83603308e-10, 0.45857957, 3.74498077e-09, 0.888653398)
         wait(.5)
         
         local args = {
             [1] = "ProQuestProgress",
             [2] = "GetTorch"
         }
      
         game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
         local toolname = "Torch" -- replace with the name of the tool
         local Plr = game:GetService("Players").LocalPlayer
             pcall(function()
                 if Plr.Backpack:FindFirstChild(toolname) and Plr.Character:FindFirstChild(toolname) == nil then
                     local tool = Plr.Backpack:FindFirstChild(toolname)
                     Plr.Character.Humanoid:EquipTool(tool)
                 end
             end)
         wait(1)
         tweenteleoirtzz(Vector3.new(1113.20667, 5.04727077, 4364.80225, -0.780225277, 0, -0.625498652, 0, 1, 0, 0.625498652, 0, -0.780225277),CFrame.new(1113.20667, 5.04727077, 4364.80225, -0.780225277, 0, -0.625498652, 0, 1, 0, 0.625498652, 0, -0.780225277))
         wait(.5)
         local args = {
            [1] = "ProQuestProgress",
            [2] = "DestroyTorch"
         }
      
         game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
         local args = {
            [1] = "ProQuestProgress"
         }
      
         game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
         wait(.5)
         local args = {
            [1] = "ProQuestProgress",
            [2] = "GetCup"
         }
      
         game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
         local toolname = "Cup" -- replace with the name of the tool
         local Plr = game:GetService("Players").LocalPlayer
             pcall(function()
                 if Plr.Backpack:FindFirstChild(toolname) and Plr.Character:FindFirstChild(toolname) == nil then
                     local tool = Plr.Backpack:FindFirstChild(toolname)
                     Plr.Character.Humanoid:EquipTool(tool)
                 end
             end)
         wait(.5)
         tweenteleoirtzz(Vector3.new(1393.15234, 37.3737411, -1321.66858, 0.0851671547, -1.41589218e-09, 0.99636668, 2.91190938e-09, 1, 1.17215193e-09, -0.99636668, 2.80150059e-09, 0.0851671547),CFrame.new(1393.15234, 37.3737411, -1321.66858, 0.0851671547, -1.41589218e-09, 0.99636668, 2.91190938e-09, 1, 1.17215193e-09, -0.99636668, 2.80150059e-09, 0.0851671547))
      
         wait(.5)
         local args = {
            [1] = "ProQuestProgress",
            [2] = "FillCup",
            [3] = game:GetService("Players").LocalPlayer.Character.Cup
         }
      
         game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
         local args = {
            [1] = "ProQuestProgress"
         }
      
         game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
         wait(.5)
         ply.CFrame = CFrame.new(1457.9043, 88.277977, -1390.95496, -0.537260771, 1.63033693e-08, -0.843416214, -7.49195621e-08, 1, 6.70543372e-08, 0.843416214, 9.92140343e-08, -0.537260771)
         wait(.5)
         local args = {
            [1] = "ProQuestProgress",
            [2] = "SickMan"
         }
      
         game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
         wait(.5)
         tweenteleoirtzz(Vector3.new(-908.365845, 13.7778397, 4077.84668, -0.0465272143, 3.05009067e-08, -0.998917043, -2.55670285e-09, 1, 3.06530588e-08, 0.998917043, 3.98013533e-09, -0.0465272143),CFrame.new(-908.365845, 13.7778397, 4077.84668, -0.0465272143, 3.05009067e-08, -0.998917043, -2.55670285e-09, 1, 3.06530588e-08, 0.998917043, 3.98013533e-09, -0.0465272143))
         wait(.5)
         local args = {
            [1] = "ProQuestProgress",
            [2] = "RichSon"
         }
      
         game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
         wait(.5)
         tweenteleoirtzz(Vector3.new(-2850.20068, 7.39224768, 5354.99268),CFrame.new(-2850.20068, 7.39224768, 5354.99268))
         wait(.5)
         while wait() do 
               require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1} 
               require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework).activeController.timeToNextAttack = 100
               game:GetService'VirtualUser':CaptureController()
               game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)  
               require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1} 
               game:GetService'VirtualUser':CaptureController()
               game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
               require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1} 
               game:GetService'VirtualUser':CaptureController()
               game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
               game:GetService("Workspace").Enemies["Mob Leader [Lv. 120] [Boss]"].HumanoidRootPart.Size = Vector3.new(40,40,40)
               game:GetService("Workspace").Enemies["Mob Leader [Lv. 120] [Boss]"].HumanoidRootPart.CanCollide = false
               ply.CFrame = game:GetService("Workspace").Enemies["Mob Leader [Lv. 120] [Boss]"].HumanoidRootPart.CFrame * CFrame.new(0,0,-15)
               if game:GetService("Workspace").Enemies["Mob Leader [Lv. 120] [Boss]"].Humanoid.Health == 0 then
                  tweenteleoirtzz(Vector3.new(-908.365845, 13.7778397, 4077.84668, -0.0465272143, 3.05009067e-08, -0.998917043, -2.55670285e-09, 1, 3.06530588e-08, 0.998917043, 3.98013533e-09, -0.0465272143),CFrame.new(-908.365845, 13.7778397, 4077.84668, -0.0465272143, 3.05009067e-08, -0.998917043, -2.55670285e-09, 1, 3.06530588e-08, 0.998917043, 3.98013533e-09, -0.0465272143))
                  wait(.5)
                  local args = {
                     [1] = "ProQuestProgress",
                     [2] = "RichSon"
                  }
      
                  game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                  local args = {
                     [1] = "ProQuestProgress"
                  }
      
                  game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                  wait(.5)
                  local toolname = "Relic" -- replace with the name of the tool
                  local Plr = game:GetService("Players").LocalPlayer
                  pcall(function()
                     if Plr.Backpack:FindFirstChild(toolname) and Plr.Character:FindFirstChild(toolname) == nil then
                        local tool = Plr.Backpack:FindFirstChild(toolname)
                        Plr.Character.Humanoid:EquipTool(tool)
                     end
                  end)
                  tweenteleoirtzz(Vector3.new(-1405.45728, 29.8778057, 4.69083405, 0.87234509, 1.10293916e-08, 0.488890588, -2.06415529e-09, 1, -1.88768947e-08, -0.488890588, 1.54580206e-08, 0.87234509),CFrame.new(-1405.45728, 29.8778057, 4.69083405, 0.87234509, 1.10293916e-08, 0.488890588, -2.06415529e-09, 1, -1.88768947e-08, -0.488890588, 1.54580206e-08, 0.87234509))
                  wait(.5)
      
                  local args = {
                     [1] = "ProQuestProgress",
                     [2] = "PlaceRelic"
                  }
      
                  game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                  local args = {
                     [1] = "ProQuestProgress"
                  }
      
                  game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                  require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1} 
                  require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework).activeController.timeToNextAttack = 100
                  game:GetService'VirtualUser':CaptureController()
                  game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)  
                  require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1} 
                  game:GetService'VirtualUser':CaptureController()
                  game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
                  require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1} 
                  game:GetService'VirtualUser':CaptureController()
                  game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
                  game:GetService("Workspace").Enemies["Saber Expert [Lv. 200] [Boss]"].HumanoidRootPart.Size = Vector3.new(40,40,40)
                  game:GetService("Workspace").Enemies["Saber Expert [Lv. 200] [Boss]"].HumanoidRootPart.CanCollide = false
                  ply.CFrame = game:GetService("Workspace").Enemies["Saber Expert [Lv. 200] [Boss]"].HumanoidRootPart.CFrame * CFrame.new(0,0,-15)
               end
         end
      end
   else
      tweenteleoirtzz(Vector3.new(ply.CFrame))
   end
end)

Main2:addToggle("Factory", nil, function(value)
   _G.Factory = value
end)
Main2:addToggle("Auto Superhuman",nil,function(value)
_G.Superhuman = value
end)

Main2:addToggle("Auto DeathStep",nil,function(value)
_G.DeathStep = value
end)

Main2:addToggle("Auto Electric Claw",nil,function(value)
_G.Electro = value
end)

Main2:addToggle("Auto Elite Hunter",nil,function(value)
_G.elitehunt = value
end)
Main2:addToggle("Auto Buy Legendary Sword",nil,function(value)
_G.BuySwordLegendary = value
end)

Main2:addToggle("Auto Buy Haki Color",nil,function(value)
_G.BuyHakiColorsDealer = value
end)
Main2:addToggle("Auto Buy Random Bone",nil,function(value)
_G.AutoBuyRandombone = value

while _G.AutoBuyRandombone do wait()
   pcall(function()
   local args = {
      [1] = "Bones",
      [2] = "Buy",
      [3] = 1,
      [4] = 1
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   end)
end
end)
_G.done = false
Main2:addToggle("Auto HallowScythe",nil,function(value)
_G.AutoFarmBossHallow = value
while _G.AutoFarmBossHallow do wait()
   pcall(function()
   if game:GetService("Workspace").Enemies:FindFirstChild("Soul Reaper [Lv. 2100] [Raid Boss]") then
      for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
         if string.find(v.Name , "Soul Reaper") then
            repeat wait()
               itemequip(weapongg)
               local Distancex = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
               local Speexd = 100 -- ความเร็วของมึง
               tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
               tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,15,8)})
               tweenx:Play()
               v.HumanoidRootPart.Size = Vector3.new(40,40,40)
               v.HumanoidRootPart.Transparency = 0.85
               v.HumanoidRootPart.CanCollide = true
               v.Humanoid.WalkSpeed = 0
               v.Humanoid:ChangeState(11)
               click()
            until v.Humanoid.Health <= 0 or _G.AutoFarmBossHallow == false
         end
      end
   else
      if game:GetService("ReplicatedStorage"):FindFirstChild("Soul Reaper [Lv. 2100] [Raid Boss]") then
         local Distancex = (game:GetService("ReplicatedStorage"):FindFirstChild("Soul Reaper [Lv. 2100] [Raid Boss]").HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
         local Speexd = 100 -- ความเร็วของมึง
         tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
         tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("ReplicatedStorage"):FindFirstChild("Soul Reaper [Lv. 2100] [Raid Boss]").HumanoidRootPart.CFrame})
         tweenx:Play()
         wait(Distancex/Speexd)
      else
         if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Hallow Essence") then
            itemequip("Hallow Essence")
            local Distancex = (Vector3.new(-8932.322265625, 146.83154296875, 6062.55078125) - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
            local Speexd = 100 -- ความเร็วของมึง
            tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
            tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(-8932.322265625, 146.83154296875, 6062.55078125)})
            tweenx:Play()
            wait(Distancex/Speexd)
         end
      end
   end
   end)
end
end)
Main2:addToggle("Auto Store Fruit All",nil,function(value)
_G.AutoStoreFruitAll = value
while _G.AutoStoreFruitAll do wait()
   pcall(function()
   if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bomb Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bomb Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Bomb-Bomb")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spike Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spike Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Spike-Spike")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Chop Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Chop Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Chop-Chop")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spring Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spring Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Spring-Spring")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Kilo Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Kilo Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Kilo-Kilo")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Smoke Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Smoke Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Smoke-Smoke")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Spin Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Spin Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Spin-Spin")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flame Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flame Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Flame-Flame")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bird: Falcon Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bird: Falcon Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Bird-Bird: Falcon")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Ice Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Ice Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Ice-Ice")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sand Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Sand Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Sand-Sand")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dark Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dark Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Dark-Dark")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Diamond Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Diamond Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Diamond-Diamond")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Light Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Light Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Light-Light")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Love Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Love Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Love-Love")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Rubber Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Rubber Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Rubber-Rubber")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Barrier Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Barrier Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Barrier-Barrier")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Magma Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Magma Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Magma-Magma")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Door Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Door Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Door-Door")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Quake Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Quake Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Quake-Quake")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Human-Human: Buddha Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Human-Human: Buddha Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Human-Human: Buddha")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("String Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("String Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","String-String")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Bird: Phoenix Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Bird: Phoenix Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Bird-Bird: Phoenix")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Rumble Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Rumble Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Rumble-Rumble")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Paw Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Paw Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Paw-Paw")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Gravity Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Gravity Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Gravity-Gravity")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dough Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dough Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Dough-Dough")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Venom Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Venom Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Venom-Venom")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Control Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Control Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Control-Control")
   elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dragon Fruit") or game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Dragon Fruit") then
      game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit","Dragon-Dragon")
   end
   end)
end
end)

function tweenteleoirtpower(XXXXx,Arfggg)
   local Distance = (XXXXx - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
   local Speed = 149
   game:GetService("TweenService"):Create(
   game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart,
   TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear),
   {CFrame = Arfggg}
   ):Play()
   _G.NoClip = true
   wait(Distance/Speed)
   _G.NoClip = false
end

spawn(function()
   while wait() do
       if _G.Factory then
           pcall(function()
               for i,v in pairs(game:GetService("Workspace").Map.Dressrosa.SmileFactory:GetChildren()) do
                   if v.Name == "Core" then
                       repeat wait()
                           if _G.Factory == true then
                               _G.AutoFarm = false
                           elseif _G.Factory == false then
                               _G.AutoFarm = true
                           end
                           v.HumanoidRootPart.Size = Vector3.new(60,60,60)
                           v.HumanoidRootPart.Transparency = 1
                           v.HumanoidRootPart.CanCollide = false
                           game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(25, 0, 7)
                           if sethiddenproperty then
                               sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
                           end
                       until v.Humanoid.Health == 0 or not _G.Factory
                   else
                     tweenteleoirtzz(Vector3.new(438.675537, 209.555679, -431.071808, 0.988916099, 1.77239485e-08, -0.148475274, -2.25331185e-08, 1, -3.07082537e-08, 0.148475274, 3.37134978e-08, 0.988916099),CFrame.new(438.675537, 209.555679, -431.071808, 0.988916099, 1.77239485e-08, -0.148475274, -2.25331185e-08, 1, -3.07082537e-08, 0.148475274, 3.37134978e-08, 0.988916099))
                   end
               end
           end)
       end
   end
end)
spawn(function()
   while wait() do
       if _G.Factory then
           pcall(function()
               require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1} 
               require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework).activeController.timeToNextAttack = 100
               game:GetService'VirtualUser':CaptureController()
               game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)  
               require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1} 
               game:GetService'VirtualUser':CaptureController()
               game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
               require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1} 
               game:GetService'VirtualUser':CaptureController()
               game:GetService('VirtualUser'):ClickButton1(Vector2.new(851, 158), game:GetService("Workspace").Camera.CFrame)
           end)
       end
   end
end)
spawn(function()
   while wait() do
       if _G.Factory then
           pcall(function ()
               EquipWeapon(ToolName)
           end)
       end
   end
end)
local AutoStats = powerx:addPage("Auto-Stats", 7040410130)
local AutoStats =  AutoStats:addSection("Auto Stats ")



_G.STATSUPPOINT = 3

AutoStats:addToggle("Melee", nil, function(value)
_G.UPMELEE = value
while _G.UPMELEE do wait()
local args = {
    [1] = "AddPoint",
    [2] = "Melee",
    [3] = _G.STATSUPPOINT
}

game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end
end)

AutoStats:addToggle("Defense", nil, function(value)
_G.UPDEFENDS = value
while _G.UPDEFENDS do wait()
local args = {
    [1] = "AddPoint",
    [2] = "Defense",
    [3] = _G.STATSUPPOINT
}

game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end
end)

AutoStats:addToggle("Sword", nil, function(value)
   _G.UPSWORD = value
   while _G.UPSWORD do wait()
   local args = {
       [1] = "AddPoint",
       [2] = "Sword",
       [3] = _G.STATSUPPOINT
   }
   
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   end
end)

AutoStats:addToggle("Gun", nil, function(value)
   _G.UPGUN = value
   while _G.UPGUN do wait()
   local args = {
       [1] = "AddPoint",
       [2] = "Gun",
       [3] = _G.STATSUPPOINT
   }
   
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   end
end)

AutoStats:addToggle("Demon Fruit", nil, function(value)
   _G.UPDEMONFRUIT = value
   while _G.UPDEMONFRUIT do wait()
      game:GetService("ReplicatedStorage").Remotes["CommF_"]:InvokeServer("AddPoint", "Demon Fruit", _G.STATSUPPOINT)
   end
end)



AutoStats:addSlider("Slider", 3, 1, 100, function(value)
_G.STATSUPPOINT = value
end)
   

function click()
   game:GetService'VirtualUser':CaptureController()
   game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
end


local Teleport = powerx:addPage("Teleport", 7044226690)
local Teleport =  Teleport:addSection("Teleport ")

function tweenteleoirtzz(XXXXx,Arfggg)
   local Distance = (XXXXx - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
   local Speed = 149
   game:GetService("TweenService"):Create(
   game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart,
   TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear),
   {CFrame = Arfggg}
   ):Play()
   _G.NoClip = true
   wait(Distance/Speed)
   _G.NoClip = false
end
if OldWorld then
   Teleport:addButton("Start Island",function()
   tweenteleoirtzz(Vector3.new(1071.2832, 16.3085976, 1426.86792),CFrame.new(1071.2832, 16.3085976, 1426.86792))
   end)
   Teleport:addButton("Marine Start",function()
   tweenteleoirtzz(Vector3.new(-2573.3374, 6.88881969, 2046.99817),CFrame.new(-2573.3374, 6.88881969, 2046.99817))
   end)
   Teleport:addButton("Middle Town",function()
   tweenteleoirtzz(Vector3.new(-655.824158, 7.88708115, 1436.67908),CFrame.new(-655.824158, 7.88708115, 1436.67908))
   end)
   Teleport:addButton("Jungle",function()
   tweenteleoirtzz(Vector3.new(-1249.77222, 11.8870859, 341.356476),CFrame.new(-1249.77222, 11.8870859, 341.356476))
   end)
   Teleport:addButton("Pirate Village",function()
   tweenteleoirtzz(Vector3.new(-1122.34998, 4.78708982, 3855.91992),CFrame.new(-1122.34998, 4.78708982, 3855.91992))
   end)
   Teleport:addButton("Desert",function()
   tweenteleoirtzz(Vector3.new(1094.14587, 6.47350502, 4192.88721),CFrame.new(1094.14587, 6.47350502, 4192.88721))
   end)
   Teleport:addButton("Frozen Village",function()
   tweenteleoirtzz(Vector3.new(1198.00928, 27.0074959, -1211.73376),CFrame.new(1198.00928, 27.0074959, -1211.73376))
   end)
   Teleport:addButton("MarineFord",function()
   tweenteleoirtzz(Vector3.new(-4505.375, 20.687294, 4260.55908),CFrame.new(-4505.375, 20.687294, 4260.55908))
   end)
   Teleport:addButton("Colosseum",function()
   tweenteleoirtzz(Vector3.new(-1428.35474, 7.38933945, -3014.37305),CFrame.new(-1428.35474, 7.38933945, -3014.37305))
   end)
   Teleport:addButton("Sky 1st Floor",function()
   tweenteleoirtzz(Vector3.new(-4970.21875, 717.707275, -2622.35449),CFrame.new(-4970.21875, 717.707275, -2622.35449))
   end)
   Teleport:addButton("Sky 2st Floor",function()
   tweenteleoirtzz(Vector3.new(-4813.0249, 903.708557, -1912.69055),CFrame.new(-4813.0249, 903.708557, -1912.69055))
   end)
   Teleport:addButton("Sky 3st Floor",function()
   tweenteleoirtzz(Vector3.new(-7952.31006, 5545.52832, -320.704956),CFrame.new(-7952.31006, 5545.52832, -320.704956))
   end)
   Teleport:addButton("Prison",function()
   tweenteleoirtzz(Vector3.new(4854.16455, 5.68742752, 740.194641),CFrame.new(4854.16455, 5.68742752, 740.194641))
   end)
   Teleport:addButton("Magma Village",function()
   tweenteleoirtzz(Vector3.new(-5231.75879, 8.61593437, 8467.87695),CFrame.new(-5231.75879, 8.61593437, 8467.87695))
   end)
   Teleport:addButton("UndeyWater City",function()
   tweenteleoirtzz(Vector3.new(61163.8516, 11.7796879, 1819.78418),CFrame.new(61163.8516, 11.7796879, 1819.78418))
   end)
   Teleport:addButton("Fountain City",function()
   tweenteleoirtzz(Vector3.new(5132.7124, 4.53632832, 4037.8562),CFrame.new(5132.7124, 4.53632832, 4037.8562))
   end)
   Teleport:addButton("House Cyborg's",function()
   tweenteleoirtzz(Vector3.new(6262.72559, 71.3003616, 3998.23047),CFrame.new(6262.72559, 71.3003616, 3998.23047))
   end)
   Teleport:addButton("Shank's Room",function()
   tweenteleoirtzz(Vector3.new(-1442.16553, 29.8788261, -28.3547478),CFrame.new(-1442.16553, 29.8788261, -28.3547478))
   end)
   Teleport:addButton("Mob Island",function()
   tweenteleoirtzz(Vector3.new(-2850.20068, 7.39224768, 5354.99268),CFrame.new(-2850.20068, 7.39224768, 5354.99268))
   end)
end
if Sea2 then
   Teleport:addButton("Dock",function()
   tweenteleoirtzz(Vector3.new(82.9490662, 18.0710983, 2834.98779),CFrame.new(82.9490662, 18.0710983, 2834.98779))
   end)
   Teleport:addButton("Kingdom of Rose",function()
   tweenteleoirtzz(Vector3.new(-394.983521, 118.503128, 1245.8446),CFrame.new(-394.983521, 118.503128, 1245.8446))
   end)
   Teleport:addButton("Mansion",function()
   tweenteleoirtzz(Vector3.new(-390.096313, 331.886475, 673.464966),CFrame.new(-390.096313, 331.886475, 673.464966))
   end)
   Teleport:addButton("Flamingo Room",function()
   tweenteleoirtzz(Vector3.new(2302.19019, 15.1778421, 663.811035),CFrame.new(2302.19019, 15.1778421, 663.811035))
   end)
   Teleport:addButton("Green Zone",function()
   tweenteleoirtzz(Vector3.new(-2372.14697, 72.9919434, -3166.51416),CFrame.new(-2372.14697, 72.9919434, -3166.51416))
   end)
   Teleport:addButton("Cafe",function()
   tweenteleoirtzz(Vector3.new(-385.250916, 73.0458984, 297.388397),CFrame.new(-385.250916, 73.0458984, 297.388397))
   end)
   Teleport:addButton("Factroy",function()
   tweenteleoirtzz(Vector3.new(430.42569, 210.019623, -432.504791),CFrame.new(430.42569, 210.019623, -432.504791))
   end)
   Teleport:addButton("Colosseum",function()
   tweenteleoirtzz(Vector3.new(-1836.58191, 44.5890656, 1360.30652),CFrame.new(-1836.58191, 44.5890656, 1360.30652))
   end)
   Teleport:addButton("GraveIsland",function()
   tweenteleoirtzz(Vector3.new(-5411.47607, 48.8234024, -721.272522),CFrame.new(-5411.47607, 48.8234024, -721.272522))
   end)
   Teleport:addButton("Snow Mountain",function()
   tweenteleoirtzz(Vector3.new(511.825226, 401.765198, -5380.396),CFrame.new(511.825226, 401.765198, -5380.396))
   end)
   Teleport:addButton("Cold Island",function()
   tweenteleoirtzz(Vector3.new(-6026.96484, 14.7461271, -5071.96338),CFrame.new(-6026.96484, 14.7461271, -5071.96338))
   end)
   Teleport:addButton("Hot Island",function()
   tweenteleoirtzz(Vector3.new(-5478.39209, 15.9775667, -5246.9126),CFrame.new(-5478.39209, 15.9775667, -5246.9126))
   end)
   Teleport:addButton("Cursed Ship",function()
   tweenteleoirtzz(Vector3.new(902.059143, 124.752518, 33071.8125),CFrame.new(902.059143, 124.752518, 33071.8125))
   end)
   Teleport:addButton("IceCastle",function()
   tweenteleoirtzz(Vector3.new(5400.40381, 28.21698, -6236.99219),CFrame.new(5400.40381, 28.21698, -6236.99219))
   end)
   Teleport:addButton("Forgotten Island",function()
   tweenteleoirtzz(Vector3.new(-3043.31543, 238.881271, -10191.5791),CFrame.new(-3043.31543, 238.881271, -10191.5791))
   end)
   Teleport:addButton("Usoapp Island",function()
   tweenteleoirtzz(Vector3.new(4748.78857, 8.35370827, 2849.57959),CFrame.new(4748.78857, 8.35370827, 2849.57959))
   end)
   Teleport:addButton("Minisky Island",function()
   tweenteleoirtzz(Vector3.new(-260.358917, 49325.7031, -35259.3008),CFrame.new(-260.358917, 49325.7031, -35259.3008))
   end)
end
if ThreeWorld then
   Teleport:addButton("Port Towen",function()
   tweenteleoirtzz(Vector3.new(-610.309692, 57.8323097, 6436.33594),CFrame.new(-610.309692, 57.8323097, 6436.33594))
   end)
   Teleport:addButton("Hydra Island",function()
   tweenteleoirtzz(Vector3.new(5229.99561, 603.916565, 345.154022),CFrame.new(5229.99561, 603.916565, 345.154022, -0.137452736))
   end)
   Teleport:addButton("Great Tree",function()
   tweenteleoirtzz(Vector3.new(2174.94873, 28.7312393, -6728.83154),CFrame.new(2174.94873, 28.7312393, -6728.83154))
   end)
   Teleport:addButton("Castle on the Sea",function()
   tweenteleoirtzz(Vector3.new(-5477.62842, 313.794739, -2808.4585),CFrame.new(-5477.62842, 313.794739, -2808.4585))
   end)
   Teleport:addButton("Floating Turtle",function()
   tweenteleoirtzz(Vector3.new(-10919.2998, 331.788452, -8637.57227),CFrame.new(-10919.2998, 331.788452, -8637.57227))
   end)
   Teleport:addButton("Mansion",function()
   tweenteleoirtzz(Vector3.new(-12553.8125, 332.403961, -7621.91748),CFrame.new(-12553.8125, 332.403961, -7621.91748))
   end)
   Teleport:addButton("Secret Temple",function()
   tweenteleoirtzz(Vector3.new(5217.35693, 6.56511116, 1100.88159, 0.00408430398),CFrame.new(5217.35693, 6.56511116, 1100.88159, 0.00408430398))
   end)
   Teleport:addButton("Friendly Arena",function()
   tweenteleoirtzz(Vector3.new(5220.28955, 72.8193436, -1450.86304),CFrame.new(5220.28955, 72.8193436, -1450.86304))
   end)
   Teleport:addButton("Beautiful Pirate Domain",function()
   tweenteleoirtzz(Vector3.new(5310.8095703125, 21.594484329224, 129.39053344727),CFrame.new(5310.8095703125, 21.594484329224, 129.39053344727))
   end)
   Teleport:addButton("Haunted Castle",function()
   tweenteleoirtzz(Vector3.new(-9506.1064453125, 142.13989257813, 5526.0405273438),CFrame.new(-9506.1064453125, 142.13989257813, 5526.0405273438))
   end)
end

local Raid = powerx:addPage("Auto Raid", 7251993295)
local Raid =  Raid:addSection("Auto Raid ")


Raid:addToggle(" Kill Aura [ Raid ] [ Beta ] ",nil,function(value)
_G.killaurxaxx = value
while _G.killaurxaxx do wait()
   pcall(function()
   for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
      if v.ClassName == "Model" then
         v.Humanoid.Health =  die
      end
   end
   end)
end
end)

if Sea2 then

   Raid:addToggle(" Auto Next Island [ Raid ]",nil,function(value)
   _G.NextIsland = value
   while _G.NextIsland do wait()
      pcall(function()
      game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
      if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
         tweenteleoirtzz(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame * CFrame.new(0,40,0))
      elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
         tweenteleoirtzz(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame * CFrame.new(0,40,0))
      elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
         tweenteleoirtzz(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame * CFrame.new(0,40,0))
      elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
         tweenteleoirtzz(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame * CFrame.new(0,40,0))
      elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
         tweenteleoirtzz(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame * CFrame.new(0,40,0))
      end
      end)
   end
   end)
end
if ThreeWorld then

   Raid:addToggle(" Auto Next Island [ Raid ]",nil,function(value)
   _G.NextIsland = value
   while _G.NextIsland do wait()
      pcall(function()
      game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
      if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
         tweenteleoirtzz(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame * CFrame.new(0,360,0))
      elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
         tweenteleoirtzz(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame * CFrame.new(0,360,0))
      elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
         tweenteleoirtzz(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame * CFrame.new(0,360,0))
      elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
         tweenteleoirtzz(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame * CFrame.new(0,360,0))
      elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
         tweenteleoirtzz(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame * CFrame.new(0,360,0))
      end
      end)
   end
   end)
end
if Sea2 then
   Raid:addButton("Teleport to Lab",function()
   tweenteleoirtzz(Vector3.new(-6438.73535, 250.645355, -4501.50684),CFrame.new(-6438.73535, 250.645355, -4501.50684))
   end)
end
if ThreeWorld then
   Raid:addButton("Teleport to Lab",function()
   tweenteleoirtzz(Vector3.new(-5017.40869, 314.844055, -2823.0127, -0.925743818, 4.48217499e-08, -0.378151238, 4.55503146e-09, 1, 1.07377559e-07, 0.378151238, 9.7681621e-08, -0.925743818),CFrame.new(-5017.40869, 314.844055, -2823.0127, -0.925743818, 4.48217499e-08, -0.378151238, 4.55503146e-09, 1, 1.07377559e-07, 0.378151238, 9.7681621e-08, -0.925743818))
   end)
end



local ZXXZZ = powerx:addPage("Player", 7252023075)
local ZXXZZ =  ZXXZZ:addSection("Player ")

ply = {}
for i,v in pairs(game.Players:GetPlayers()) do
   table.insert(ply, v.Name)
end

ZXXZZ:addDropdown("Select Player", ply, function(list)
dinoply = list
end)

ZXXZZ:addButton("Refresh Player", function()
table.clear(ply)
for i,v in pairs(game.Players:GetPlayers()) do
   table.insert(ply, v.Name)
end
end)

ZXXZZ:addButton("Teleport To Player", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players[dinoply].Character.HumanoidRootPart.CFrame
end)

ZXXZZ:addToggle("Auto Bounty [ Gun Only! ]", function(State)
_G.RQIO = State
while _G.RQIO do wait()
   pcall(function()
   for i, v in pairs(game:GetService("Workspace").Characters:GetChildren()) do
      if v.Name == dinoply then
         equipgun()
         local magnitude = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
         if magnitude < 1000 then
            local Distancex = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
            local Speexd = 1000 -- ความเร็วของมึง
            tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
            tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = v.HumanoidRootPart.CFrame*CFrame.new(0,15,8)})
            tweenx:Play()
            wait(Distancex/Speexd)
            v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
            local args = {
               [1] = game:GetService("Players"):FindFirstChild(v.Name).Character.HumanoidRootPart.Position,
               [2] = game:GetService("Players"):FindFirstChild(v.Name).Character.HumanoidRootPart
            }
            game:GetService("Players").LocalPlayer.Character[gunname()].RemoteFunctionShoot:InvokeServer(unpack(args))
         else
            local Distancex = (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
            local Speexd = 150 -- ความเร็วของมึง
            tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
            tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = v.HumanoidRootPart.CFrame*CFrame.new(0,30,0)})
            tweenx:Play()
            wait(Distancex/Speexd)
         end
      end
   end
   end)
end
end)



local Localplayer = powerx:addPage("localplayer", 7252023075)
local Localplayer =  Localplayer:addSection("Character")
Localplayer:addToggle("Auto Click",false,function(value)
   AuctoClick = value
end)
spawn(function()
   while wait(.1) do
       if AuctoClick then
           Click()
       end
   end
end)
Fly = false
function activatefly()
   local mouse=game.Players.LocalPlayer:GetMouse''
   localplayer=game.Players.LocalPlayer
   game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")
   local torso = game.Players.LocalPlayer.Character.HumanoidRootPart
   local speed=180
   local keys={a=false,d=false,w=false,s=false}
   local e1
   local e2
   local function start()
       local pos = Instance.new("BodyPosition",torso)
       local gyro = Instance.new("BodyGyro",torso)
       pos.Name="EPIXPOS"
       pos.maxForce = Vector3.new(math.huge, math.huge, math.huge)
       pos.position = torso.Position
       gyro.maxTorque = Vector3.new(9e9, 9e9, 9e9)
       gyro.cframe = torso.CFrame
       repeat
           wait()
           localplayer.Character.Humanoid.PlatformStand=true
           local new=gyro.cframe - gyro.cframe.p + pos.position
           if not keys.w and not keys.s and not keys.a and not keys.d then
               speed=3
           end
           if keys.w then
               new = new + workspace.CurrentCamera.CoordinateFrame.lookVector * speed
               speed=speed+9.02
           end
           if keys.s then
               new = new - workspace.CurrentCamera.CoordinateFrame.lookVector * speed
               speed=speed+4.02
           end
           if keys.d then
               new = new * CFrame.new(speed,0,0)
               speed=speed+2.02
           end
           if keys.a then
               new = new * CFrame.new(-speed,0,0)
               speed=speed+3.02
           end
           if speed>5 then
               speed=9.5
           end
           pos.position=new.p
           if keys.w then
               gyro.cframe = workspace.CurrentCamera.CoordinateFrame*CFrame.Angles(-math.rad(speed*15),0,0)
           elseif keys.s then
               gyro.cframe = workspace.CurrentCamera.CoordinateFrame*CFrame.Angles(math.rad(speed*15),0,0)
           else
               gyro.cframe = workspace.CurrentCamera.CoordinateFrame
           end
       until not Fly
       if gyro then
           gyro:Destroy()
       end
       if pos then
           pos:Destroy()
       end
       flying=false
       localplayer.Character.Humanoid.PlatformStand=false
       speed=5
   end
   e1=mouse.KeyDown:connect(function(key)
       if not torso or not torso.Parent then
           flying=false e1:disconnect() e2:disconnect() return
       end
       if key=="w" then
           keys.w=true
       elseif key=="s" then
           keys.s=true
       elseif key=="a" then
           keys.a=true
       elseif key=="d" then
           keys.d=true
       end
   end)
   e2=mouse.KeyUp:connect(function(key)
       if key=="w" then
           keys.w=false
       elseif key=="s" then
           keys.s=false
       elseif key=="a" then
           keys.a=false
       elseif key=="d" then
           keys.d=false
       end
   end)
   start()
end
Localplayer:addToggle("Fly",false,function(Value)
   Fly = Value
   activatefly()
end)
Localplayer:addToggle("No Clip",false,function(value)
   NoClip = value
end)
game:GetService("RunService").Heartbeat:Connect(
function()
   if NoClip or _G.Pole or _G.SwanGlasses then
       game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
   end
end)
Localplayer:addToggle("Dodge No Cooldown",false,function(Value)
   nododgecool = Value
   NoDodgeCool()
end)
Localplayer:addToggle("Infinits Energy",false,function(value)
   InfinitsEnergy = value
   originalstam = LocalPlayer.Character.Energy.Value
end)
local LocalPlayer = game:GetService'Players'.LocalPlayer
local originalstam = LocalPlayer.Character.Energy.Value
function infinitestam()
   LocalPlayer.Character.Energy.Changed:connect(function()
       if InfinitsEnergy then
           LocalPlayer.Character.Energy.Value = originalstam
       end
   end)
end
spawn(function()
   while wait(.1) do
       if InfinitsEnergy then
           wait(0.3)
           originalstam = LocalPlayer.Character.Energy.Value
           infinitestam()
       end
   end
end)
function infAb()
   if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
       game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
   end
   if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
       game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
   end
   if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
       game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
   end
   if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
       game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
   end
   wait(.1)
   local inf = Instance.new("ParticleEmitter")
   inf.Acceleration = Vector3.new(0,0,0)
   inf.Archivable = true
   inf.Drag = 20
   inf.EmissionDirection = Enum.NormalId.Top
   inf.Enabled = true
   inf.Lifetime = NumberRange.new(0.2,0.2)
   inf.LightInfluence = 0
   inf.LockedToPart = true
   inf.Name = "Agility"
   inf.Rate = 500
   local numberKeypoints2 = {
       NumberSequenceKeypoint.new(0, 0);  -- At t=0, size of 0
       NumberSequenceKeypoint.new(1, 4); -- At t=1, size of 10
   }

   inf.Size = NumberSequence.new(numberKeypoints2)
   inf.RotSpeed = NumberRange.new(999, 9999)
   inf.Rotation = NumberRange.new(0, 0)
   inf.Speed = NumberRange.new(30, 30)
   inf.SpreadAngle = Vector2.new(360,360)
   inf.Texture = ""
   inf.VelocityInheritance = 0
   inf.ZOffset = 2
   inf.Transparency = NumberSequence.new(0)
   inf.Color = ColorSequence.new(Color3.fromRGB(0, 255, 255),Color3.fromRGB(0, 255, 255))
   inf.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart

   local inf2 = Instance.new("ParticleEmitter")
   inf2.Acceleration = Vector3.new(0,0,0)
   inf2.Archivable = true
   inf2.Drag = 20
   inf2.EmissionDirection = Enum.NormalId.Top
   inf2.Enabled = true
   inf2.Lifetime = NumberRange.new(0.2,0.2)
   inf2.LightInfluence = 0
   inf2.LockedToPart = true
   inf2.Name = "Agility"
   local numberKeypoints3 = {
       NumberSequenceKeypoint.new(0, 0);  -- At t=0, size of 0
       NumberSequenceKeypoint.new(1, 4); -- At t=1, size of 10
   }

   inf2.Size = NumberSequence.new(numberKeypoints3)
   inf2.Rate = 500
   inf2.RotSpeed = NumberRange.new(999, 9999)
   inf2.Rotation = NumberRange.new(0, 0)
   inf2.Speed = NumberRange.new(30, 30)
   inf2.SpreadAngle = Vector2.new(360,360)
   inf2.Texture = ""
   inf2.VelocityInheritance = 0
   inf2.Transparency = NumberSequence.new(0)
   inf2.Color = ColorSequence.new(Color3.fromRGB(255, 0, 0),Color3.fromRGB(255, 0, 0))
   inf2.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart

   local inf3 = Instance.new("ParticleEmitter")
   inf3.Acceleration = Vector3.new(0,0,0)
   inf3.Archivable = true
   inf3.Drag = 20
   inf3.EmissionDirection = Enum.NormalId.Top
   inf3.Enabled = true
   inf3.Lifetime = NumberRange.new(0.2,0.2)
   inf3.LightInfluence = 0
   inf3.LockedToPart = true
   inf3.Name = "Agility"
   local numberKeypoints4 = {
       NumberSequenceKeypoint.new(0, 0);  -- At t=0, size of 0
       NumberSequenceKeypoint.new(1, 4); -- At t=1, size of 10
   }

   inf3.Size = NumberSequence.new(numberKeypoints4)
   inf3.Rate = 500
   inf3.RotSpeed = NumberRange.new(999, 9999)
   inf3.Rotation = NumberRange.new(0, 0)
   inf3.Speed = NumberRange.new(30, 30)
   inf3.SpreadAngle = Vector2.new(360,360)
   inf3.Texture = ""
   inf3.VelocityInheritance = 0
   inf3.Transparency = NumberSequence.new(0)
   inf3.Color = ColorSequence.new(Color3.fromRGB(255, 255, 0),Color3.fromRGB(255, 255, 0))
   inf3.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart

   local inf4 = Instance.new("ParticleEmitter")
   inf4.Acceleration = Vector3.new(0,0,0)
   inf4.Archivable = true
   inf4.Drag = 20
   inf4.EmissionDirection = Enum.NormalId.Top
   inf4.Enabled = true
   inf4.Lifetime = NumberRange.new(0.2,0.2)
   inf4.LightInfluence = 0
   inf4.LockedToPart = true
   inf4.Name = "Agility"
   local numberKeypoints5 = {
       NumberSequenceKeypoint.new(0, 0);  -- At t=0, size of 0
       NumberSequenceKeypoint.new(1, 4); -- At t=1, size of 10
   }

   inf4.Size = NumberSequence.new(numberKeypoints5)
   inf4.Rate = 500
   inf4.RotSpeed = NumberRange.new(999, 9999)
   inf4.Rotation = NumberRange.new(0, 0)
   inf4.Speed = NumberRange.new(30, 30)
   inf4.SpreadAngle = Vector2.new(360,360)
   inf4.Texture = ""
   inf4.VelocityInheritance = 0
   inf4.Transparency = NumberSequence.new(0)
   inf4.Color = ColorSequence.new(Color3.fromRGB(255, 255, 255),Color3.fromRGB(255, 6, 60))
   inf4.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
end

Localplayer:addToggle("Inf Ability",false,function(inf)
   if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
       game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
   end
   if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
       game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
   end
   if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
       game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
   end
   if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
       game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
   end
   wait()
   getgenv().InfAbility = inf
end)

spawn(function()
   while wait(1) do
       pcall(function()
           if InfAbility then
               if not game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
                   if InfAbility == true then
                       infAb()
                   elseif InfAbility == false then
                       if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
                           game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
                       end
                       if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
                           game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
                       end
                       if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
                           game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
                       end
                       if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
                           game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
                       end
                   else
                       if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
                           game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
                       end
                       if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
                           game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
                       end
                       if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
                           game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
                       end
                       if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
                           game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
                       end
                   end
               end
           end
       end)
   end
end)
Localplayer:addToggle("Invisble My Character",nil,function(value)
   _G.invme = value
   while _G.invme do wait()
      pcall(function()
      for i,v in pairs(game:GetService("Players").LocalPlayer.Character:GetDescendants()) do
         if v.ClassName == "MeshPart" then
            v.Transparency = 1
         end
      end
      for i,v in pairs(game:GetService("Players").LocalPlayer:GetDescendants()) do
         if v.Name == "Head" then
            v.Transparency = 1
         end
      end
      for i,v in pairs(game:GetService("Players").LocalPlayer:GetDescendants()) do
         if v.ClassName == "Accessory" then
            v.Handle.Transparency = 1
         end
      end
      for i,v in pairs(game:GetService("Players").LocalPlayer:GetDescendants()) do
         if v.ClassName == "Decal" then
            v.Transparency = 1
         end
      end
      end)
   end
end)
Localplayer:addToggle("Dodge No Cooldown",nil,function(value)
   _G.nododgecool = value
   end)
Localplayer:addToggle("Inf Stamina",nil,function(value)
   InfinitsEnergy = value
   originalstam = LocalPlayer.Character.Energy.Value
end)

local XDDD = powerx:addPage("Game", 7044233235)
local Misc =  XDDD:addSection("Misc")
local UI =  XDDD:addSection("UI")
local esp =  XDDD:addSection("Esp")
local Haki =  XDDD:addSection("Haki State")
local Fake =  XDDD:addSection("Fake Mote")


local ScreenGui = Instance.new("ScreenGui")
local TextLabel = Instance.new("TextLabel")
local UIGradient = Instance.new("UIGradient")

ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

TextLabel.Parent = ScreenGui
TextLabel.Active = true
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 1.000
TextLabel.BorderColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.Position = UDim2.new(0.424812019, 0, 0, 0)
TextLabel.Size = UDim2.new(0, 200, 0, 50)
TextLabel.Font = Enum.Font.GothamBold
TextLabel.Text = "Server Time"
TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.TextSize = 30.000
TextLabel.TextTransparency = 1
TextLabel.TextStrokeTransparency = 300.000

UIGradient.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(204, 255, 69)), ColorSequenceKeypoint.new(0.50, Color3.fromRGB(150, 240, 69)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(204, 255, 69))}
UIGradient.Parent = TextLabel

local function UpdateTime()
   local GameTime = math.floor(workspace.DistributedGameTime+0.5)
   local Hour = math.floor(GameTime/(60^2))%24
   local Minute = math.floor(GameTime/(60^1))%60
   local Second = math.floor(GameTime/(60^0))%60
   TextLabel.Text = ("Hour : "..Hour.." Minute : "..Minute.." Second : "..Second)
end

spawn(function()
   while true do
      UpdateTime()
      game:GetService("RunService").RenderStepped:Wait()
   end
end)


Misc:addToggle("Server Time",false,function(value)
   ServerTime = value
   if ServerTime == true then
      TextLabel.TextTransparency = 0
   elseif ServerTime == false then
      TextLabel.TextTransparency = 1
   end
end)


UI:addButton("Open Awakening", function()
   local args = {
       [1] = "AwakeningChanger",
       [2] = "Check"
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   game.Players.localPlayer.PlayerGui.Main.AwakeningToggler.Visible = true
end)
UI:addButton("Open Inventory", function()
   local args = {
       [1] = "getInventoryWeapons"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   game.Players.localPlayer.PlayerGui.Main.Inventory.Visible = true
end)
UI:addButton("Open Devil Shop", function()
   local args = {
       [1] = "GetFruits"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   game.Players.localPlayer.PlayerGui.Main.FruitShop.Visible = true
end)
UI:addButton("Open Color Haki", function()
   game.Players.localPlayer.PlayerGui.Main.Colors.Visible = true
end)
UI:addButton("Open Title Name", function()
   local args = {
       [1] = "getTitles"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   game.Players.localPlayer.PlayerGui.Main.Titles.Visible = true
end)

UI:addButton("Join Pirates Team", function()
   local args = {
       [1] = "SetTeam",
       [2] = "Pirates"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
   local args = {
       [1] = "BartiloQuestProgress"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   local args = {
       [1] = "Buso"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

UI:addButton("Join Marines Team", function()
   local args = {
       [1] = "SetTeam",
       [2] = "Marines"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   local args = {
       [1] = "BartiloQuestProgress"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   local args = {
       [1] = "Buso"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
function isnil(thing)
   return (thing == nil)
end
local function round(n)
   return math.floor(tonumber(n) + 0.5)
end
Number = math.random(1, 1000000)
function UpdatePlayerChams()
   for i,v in pairs(game:GetService'Players':GetChildren()) do
       pcall(function()
           if not isnil(v.Character) then
               if ESPPlayer then
                   if not isnil(v.Character.Head) and not v.Character.Head:FindFirstChild('NameEsp'..Number) then
                       local bill = Instance.new('BillboardGui',v.Character.Head)
                       bill.Name = 'NameEsp'..Number
                       bill.ExtentsOffset = Vector3.new(0, 1, 0)
                       bill.Size = UDim2.new(1,200,1,30)
                       bill.Adornee = v.Character.Head
                       bill.AlwaysOnTop = true
                       local name = Instance.new('TextLabel',bill)
                       name.Font = "GothamBold"
                       name.FontSize = "Size14"
                       name.TextWrapped = true
                       name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M')
                       name.Size = UDim2.new(1,0,1,0)
                       name.TextYAlignment = 'Top'
                       name.BackgroundTransparency = 1
                       name.TextStrokeTransparency = 0.5
                       if v.Team == game.Players.LocalPlayer.Team then
                           name.TextColor3 = Color3.new(255, 0 ,0)
                       else
                           name.TextColor3 = Color3.new(0, 0 ,255)
                       end
                   else
                       v.Character.Head['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M')
                   end
               else
                   if v.Character.Head:FindFirstChild('NameEsp'..Number) then
                       v.Character.Head:FindFirstChild('NameEsp'..Number):Destroy()
                   end
               end
           end
       end)
   end
end
function UpdateChestChams() 
   for i,v in pairs(game.Workspace:GetChildren()) do
       pcall(function()
           if string.find(v.Name,"Chest") then
               if ChestESP then
                   if string.find(v.Name,"Chest") then
                       if not v:FindFirstChild('NameEsp'..Number) then
                           local bill = Instance.new('BillboardGui',v)
                           bill.Name = 'NameEsp'..Number
                           bill.ExtentsOffset = Vector3.new(0, 1, 0)
                           bill.Size = UDim2.new(1,200,1,30)
                           bill.Adornee = v
                           bill.AlwaysOnTop = true
                           local name = Instance.new('TextLabel',bill)
                           name.Font = "GothamBold"
                           name.FontSize = "Size14"
                           name.TextWrapped = true
                           name.Size = UDim2.new(1,0,1,0)
                           name.TextYAlignment = 'Top'
                           name.BackgroundTransparency = 1
                           name.TextStrokeTransparency = 0.5
                           if v.Name == "Chest1" then
                               name.TextColor3 = Color3.fromRGB(255, 255, 255)
                               name.Text = ("Chest 1" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                           end
                           if v.Name == "Chest2" then
                               name.TextColor3 = Color3.fromRGB(255, 255, 255)
                               name.Text = ("Chest 2" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                           end
                           if v.Name == "Chest3" then
                               name.TextColor3 = Color3.fromRGB(255, 255 ,255)
                               name.Text = ("Chest 3" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                           end
                       else
                           v['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                       end
                   end
               else
                   if v:FindFirstChild('NameEsp'..Number) then
                       v:FindFirstChild('NameEsp'..Number):Destroy()
                   end
               end
           end
       end)
   end
end
function UpdateDevilChams() 
   for i,v in pairs(game.Workspace:GetChildren()) do
       pcall(function()
           if DevilFruitESP then
               if string.find(v.Name, "Fruit") then   
                   if not v.Handle:FindFirstChild('NameEsp'..Number) then
                       local bill = Instance.new('BillboardGui',v.Handle)
                       bill.Name = 'NameEsp'..Number
                       bill.ExtentsOffset = Vector3.new(0, 1, 0)
                       bill.Size = UDim2.new(1,200,1,30)
                       bill.Adornee = v.Handle
                       bill.AlwaysOnTop = true
                       local name = Instance.new('TextLabel',bill)
                       name.Font = "GothamBold"
                       name.FontSize = "Size14"
                       name.TextWrapped = true
                       name.Size = UDim2.new(1,0,1,0)
                       name.TextYAlignment = 'Top'
                       name.BackgroundTransparency = 1
                       name.TextStrokeTransparency = 0.5
                       name.TextColor3 = Color3.fromRGB(255, 255 ,255)
                       name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
                   else
                       v.Handle['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
                   end
               end
           else
               if v.Handle:FindFirstChild('NameEsp'..Number) then
                   v.Handle:FindFirstChild('NameEsp'..Number):Destroy()
               end
           end
       end)
   end
end
function UpdateFlowerChams() 
   for i,v in pairs(game.Workspace:GetChildren()) do
       pcall(function()
           if v.Name == "Flower2" or v.Name == "Flower1" then
               if FlowerESP then 
                   if not v:FindFirstChild('NameEsp'..Number) then
                       local bill = Instance.new('BillboardGui',v)
                       bill.Name = 'NameEsp'..Number
                       bill.ExtentsOffset = Vector3.new(0, 1, 0)
                       bill.Size = UDim2.new(1,200,1,30)
                       bill.Adornee = v
                       bill.AlwaysOnTop = true
                       local name = Instance.new('TextLabel',bill)
                       name.Font = "GothamBold"
                       name.FontSize = "Size14"
                       name.TextWrapped = true
                       name.Size = UDim2.new(1,0,1,0)
                       name.TextYAlignment = 'Top'
                       name.BackgroundTransparency = 1
                       name.TextStrokeTransparency = 0.5
                       name.TextColor3 = Color3.fromRGB(255, 255 ,255)
                       if v.Name == "Flower1" then 
                           name.Text = ("Blue Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                           name.TextColor3 = Color3.fromRGB(255, 255 ,255)
                       end
                       if v.Name == "Flower2" then
                           name.Text = ("Red Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                           name.TextColor3 = Color3.fromRGB(255, 255 ,255)
                       end
                   else
                       v['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                   end
               else
                   if v:FindFirstChild('NameEsp'..Number) then
                       v:FindFirstChild('NameEsp'..Number):Destroy()
                   end
               end
           end   
       end)
   end
end

esp:addToggle("ESP Player",false,function(a)
   ESPPlayer = a
   while ESPPlayer do wait()
       UpdatePlayerChams()
   end
end)
esp:addToggle("ESP Chest",false,function(a)
   ChestESP = a
   while ChestESP do wait()
       UpdateChestChams() 
   end
end)
esp:addToggle("ESP Devil Fruit",false,function(a)
   DevilFruitESP = a
   while DevilFruitESP do wait()
       UpdateDevilChams() 
   end
end)
esp:addToggle("ESP Flower",false,function(a)
   FlowerESP = a
   while FlowerESP do wait()
       UpdateFlowerChams() 
   end
end)
nododgecool = false
function NoDodgeCool()
   if nododgecool then
       for i,v in next, getgc() do
           if game.Players.LocalPlayer.Character.Dodge then
               if typeof(v) == "function" and getfenv(v).script == game.Players.LocalPlayer.Character.Dodge then
                   for i2,v2 in next, getupvalues(v) do
                       if tostring(v2) == "0.4" then
                           repeat wait(.1)
                               setupvalue(v,i2,0)
                           until not nododgecool
                       end
                   end
               end
           end
       end
   end
end



Fake:addTextbox("Fake Bouty",false,function(t)
   game:GetService("Players")["LocalPlayer"].leaderstats["Bounty/Honor"].Value = t
end)
Fake:addTextbox("Fake Beli",  false, function(t)
   game:GetService("Players")["LocalPlayer"].Data.Beli.Value = t
end)
Fake:addTextbox("Fake Level",  false, function(t)
   game:GetService("Players")["LocalPlayer"].Data.Level.Value = t
end)
Fake:addTextbox("Fake Exp ",  false, function(t)
   game:GetService("Players")["LocalPlayer"].Data.Exp.Value = t
end)
Fake:addTextbox("Fake Fragments",  false, function(t)
   game:GetService("Players")["Localplayer"].Data.Fragments.Value = t
end)
Fake:addTextbox("Fake Melee",  false, function(t)
   game:GetService("Players")["LocalPlayer"].Data.Stats.Melee.Level.Value = t
end)
Fake:addTextbox("Fake Defense",  false, function(t)
   game:GetService("Players")["localPlayer"].Data.Stats.Defense.Level.Value = t
end)
Fake:addTextbox("Fake Sword",  false, function(t)
   game:GetService("Players")["LocalPlayer"].Data.Stats.Sword.Level.Value = t
end)
Fake:addTextbox("Fake Gun",  false, function(t)
   game:GetService("Players")["LocalPlayer"].Data.Stats.Gun.Level.Value = FakeGun
end)
Fake:addTextbox("Fake Fruit",  false, function(t)
   game:GetService("Players")["LocalPlayer"].Data.Stats["Demon Fruit"].Level.Value = t
end)
Haki:addButton("Stage 0", function()
   local args = {
       [1] = "ChangeBusoStage",
       [2] = 0
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
Haki:addButton("Stage 1", function()
   local args = {
       [1] = "ChangeBusoStage",
       [2] = 1
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
Haki:addButton("Stage 2", function()
   local args = {
       [1] = "ChangeBusoStage",
       [2] = 2
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
Haki:addButton("Stage 3", function()
   local args = {
       [1] = "ChangeBusoStage",
       [2] = 3
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
Haki:addButton("Stage 4", function()
   local args = {
       [1] = "ChangeBusoStage",
       [2] = 4
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
Haki:addButton("Stage 5", function()
   local args = {
       [1] = "ChangeBusoStage",
       [2] = 5
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
Misc:addButton("Redeem All Code", function()
   function UseCode(Text)
       game:GetService("ReplicatedStorage").Remotes.Redeem:InvokeServer(Text)
   end
   UseCode("FUDD10")
   UseCode("BIGNEWS")
   UseCode("THEGREATACE")
   UseCode("SUB2NOOBMASTER123")
   UseCode("Sub2Daigrock")
   UseCode("Axiore")
   UseCode("TantaiGaming")
   UseCode("STRAWHATMAINE")
   UseCode("Sub2OfficialNoobie")
end)
local vu = game:GetService("VirtualUser")
game:GetService("Players").LocalPlayer.Idled:connect(function()
   vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
   wait(1)
   vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
end)
Misc:addButton("Remove Lave", function()
   for i,v in pairs(game.Workspace:GetDescendants()) do
       if v.Name == "Lava" then
           v:Destroy()
       end
   end
   for i,v in pairs(game.ReplicatedStorage:GetDescendants()) do
       if v.Name == "Lava" then
           v:Destroy()
       end
   end
end)
Misc:addButton("FPS Boost", function()
   local decalsyeeted = true -- Leaving this on makes games look shitty but the fps goes up by at least 20.
   local g = game
   local w = g.Workspace
   local l = g.Lighting
   local t = w.Terrain
   t.WaterWaveSize = 0
   t.WaterWaveSpeed = 0
   t.WaterReflectance = 0
   t.WaterTransparency = 0
   l.GlobalShadows = false
   l.FogEnd = 9e9
   l.Brightness = 0
   settings().Rendering.QualityLevel = "Level01"
   for i, v in pairs(g:GetDescendants()) do
       if v:IsA("Part") or v:IsA("Union") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then 
           v.Material = "Plastic"
           v.Reflectance = 0
       elseif v:IsA("Decal") or v:IsA("Texture") and decalsyeeted then
           v.Transparency = 1
       elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
           v.Lifetime = NumberRange.new(0)
       elseif v:IsA("Explosion") then
           v.BlastPressure = 1
           v.BlastRadius = 1
       elseif v:IsA("Fire") or v:IsA("SpotLight") or v:IsA("Smoke") or v:IsA("Sparkles") then
           v.Enabled = false
       elseif v:IsA("MeshPart") then
           v.Material = "Plastic"
           v.Reflectance = 0
           v.TextureID = 10385902758728957
       end
   end
   for i, e in pairs(l:GetChildren()) do
       if e:IsA("BlurEffect") or e:IsA("SunRaysEffect") or e:IsA("ColorCorrectionEffect") or e:IsA("BloomEffect") or e:IsA("DepthOfFieldEffect") then
           e.Enabled = false
       end
   end
end)
Misc:addButton("Super FPS Boost", function()
   for i,v in pairs(game.Workspace.Map:GetDescendants()) do
       if v.Name == "Tavern" or v.Name == "SmileFactory" or v.Name == "Tree" or v.Name == "Rocks" or v.Name == "PartHouse" or v.Name == "Hotel" or v.Name == "WallPiece" or v.Name == "MiddlePillars" or v.Name == "Cloud" or v.Name == "PluginGrass" or v.Name == "BigHouse" or v.Name == "SmallHouse" or v.Name == "Detail" then
           v:Destroy()
       end
   end 
   for i,v in pairs(game.ReplicatedStorage.Unloaded:GetDescendants()) do
       if v.Name == "Tavern" or v.Name == "SmileFactory" or v.Name == "Tree" or v.Name == "Rocks" or v.Name == "PartHouse" or v.Name == "Hotel" or v.Name == "WallPiece" or v.Name == "MiddlePillars" or v.Name == "Cloud" or v.Name == "PluginGrass" or v.Name == "BigHouse" or v.Name == "SmallHouse" or v.Name == "Detail" then
           v:Destroy()
       end
   end
   for i,v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
       if v:IsA("Accessory") or v.Name == "Pants" or v.Name == "Shirt" then
           v:Destroy()
       end
   end
   local decalsyeeted = true -- Leaving this on makes games look shitty but the fps goes up by at least 20.
   local g = game
   local w = g.Workspace
   local l = g.Lighting
   local t = w.Terrain
   t.WaterWaveSize = 0
   t.WaterWaveSpeed = 0
   t.WaterReflectance = 0
   t.WaterTransparency = 0
   l.GlobalShadows = false
   l.FogEnd = 9e9
   l.Brightness = 0
   settings().Rendering.QualityLevel = "Level01"
   for i, v in pairs(g:GetDescendants()) do
       if v:IsA("Part") or v:IsA("Union") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then
           v.Material = "Plastic"
           v.Reflectance = 0
       elseif v:IsA("Decal") or v:IsA("Texture") and decalsyeeted then
           v.Transparency = 1
       elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
           v.Lifetime = NumberRange.new(0)
       elseif v:IsA("Explosion") then
           v.BlastPressure = 1
           v.BlastRadius = 1
       elseif v:IsA("Fire") or v:IsA("SpotLight") or v:IsA("Smoke") or v:IsA("Sparkles") then
           v.Enabled = false
       elseif v:IsA("MeshPart") then
           v.Material = "Plastic"
           v.Reflectance = 0
           v.TextureID = 10385902758728957
       end
   end
   for i, e in pairs(l:GetChildren()) do
       if e:IsA("BlurEffect") or e:IsA("SunRaysEffect") or e:IsA("ColorCorrectionEffect") or e:IsA("BloomEffect") or e:IsA("DepthOfFieldEffect") then
           e.Enabled = false
       end
   end
end)
LockLevelValue = 2100
OldLevel = game.Players.localPlayer.Data.Level.Value
Misc:addSlider("Select Level Lock",  1, LockLevelValue,LockLevelValue,function(value)
   LockLevelValue = value
end)
Misc:addToggle("Lock Level",false,function(value)
   LockLevel = value
end)
spawn(function()
   while wait(.1) do
       if LockLevel then
           if game.Players.localPlayer.Data.Level.Value >= LockLevelValue then
               game.Players.localPlayer:Kick("\n Auto Fram Completed Level : "..game.Players.localPlayer.Data.Level.Value.."\n Old Level : "..OldLevel.."\nUsername : "..game.Players.LocalPlayer.Name)
           end
       end
   end
end)
local xxd = powerx:addPage("Buy Item", 7294901968)
local by =  xxd:addSection("abilytys")
local byStlye =  xxd:addSection("Fightingstyle")
local bySword =  xxd:addSection("Sword")
local byGun =  xxd:addSection("Gun")

by:addButton("Skyjump", function()
   local args = {
       [1] = "BuyHaki",
       [2] = "Geppo"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
by:addButton("Buso Haki", function()
   local args = {
       [1] = "BuyHaki",
       [2] = "Buso"
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
by:addButton("Soru", function()
   local args = {
       [1] = "BuyHaki",
       [2] = "Soru"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
byStlye:addButton("Black Leg", function()
   local args = {
       [1] = "BuyBlackLeg"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
byStlye:addButton("Electro", function()
   local args = {
       [1] = "BuyElectro"
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
byStlye:addButton("Fishman Karate", function()
   local args = {
       [1] = "BuyFishmanKarate"
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
byStlye:addButton("Dragon Claw", function()
   local args = {
       [1] = "BlackbeardReward",
       [2] = "DragonClaw",
       [3] = "1"
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   local args = {
       [1] = "BlackbeardReward",
       [2] = "DragonClaw",
       [3] = "2"
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
byStlye:addButton("Superhuman", function()
   local args = {
       [1] = "BuySuperhuman"
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
byStlye:addButton("Death Step", function()
   local args = {
       [1] = "BuyDeathStep"
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
byStlye:addButton("Sharkman Karate", function()
   local args = {
       [1] = "BuySharkmanKarate",
       [2] = true
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   local args = {
       [1] = "BuySharkmanKarate"
   }

   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
by:addButton("random race", function()
   local A_1 = "BlackbeardReward"
   local A_2 = "Reroll"
   local A_3 = "2"
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2, A_3)
end)
by:addButton("buy Stat refound", function()
   local A_1 = "BlackbeardReward"
   local A_2 = "Refund"
   local A_3 = "2"
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2, A_3)
end)
by:addButton("Race Ghoul", function()
   local args = {
       [1] = "Ectoplasm",
       [2] = "BuyCheck",
       [3] = 4
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   local args = {
       [1] = "Ectoplasm",
       [2] = "Change",
       [3] = 4
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
by:addButton("Race Cyborg", function()
   local args = {
       [1] = "CyborgTrainer",
       [2] = "Buy"
   }
   game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
bySword:addButton("katana", function()
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "by"
   local A_2 = "Katana"
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2)
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "by"
   local A_2 = "Katana"
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2)
end)
bySword:addButton("Cutlass", function()
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "by"
   local A_2 = "Cutlass"
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2)
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "by"
   local A_2 = "Cutlass"
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2)
end)
bySword:addButton("MidnightBlade", function()
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "Ectoplasm"
   local A_2 = "Buy"
   local A_3 = 3
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2, A_3)
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "Ectoplasm"
   local A_2 = "Buy"
   local A_3 = 3
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2, A_3)
end)
bySword:addButton("Dualkatana", function()
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "by"
   local A_2 = "Dual Katana"
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2)
end)
bySword:addButton("iron mace", function()
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "by"
   local A_2 = "Iron Mace"
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2)
end)
byGun:addButton("Bizarre Rifle", function()
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "Ectoplasm"
   local A_2 = "Buy"
   local A_3 = 1
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2, A_3)
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "Ectoplasm"
   local A_2 = "Buy"
   local A_3 = 1
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2, A_3)
end)
byGun:addButton("Sling shot", function()
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "by"
   local A_2 = "Slingshot"
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2)
end)
byGun:addButton("Musket", function()
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "by"
   local A_2 = "Musket"
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2)
end)
byGun:addButton("Flintlock", function()
   -- Script generated by R2Sv2
   -- R2Sv2 developed by Luckyxero

   local A_1 = "by"
   local A_2 = "Flintlock"
   local Event = game:GetService("ReplicatedStorage").Remotes["CommF_"]
   Event:InvokeServer(A_1, A_2)
end)
if Secondsea then
end



-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss
-----------------------bypas yesssssssssssssssssss


game:GetService("RunService").Heartbeat:Connect(function()
   if _G.RQIO == true or _G.AutoFarmAllBoss == true then
      game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
   end
   end)
   game:GetService("RunService").Heartbeat:Connect(function()
   pcall(function()
   if _G.FastAttack and (_G.AutoFarm or _G.elitehunt or _G.AutoFarmAllBoss or _G.AutoFarmBossHallow) then
      require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework).activeController.timeToNextAttack = 0
      game:GetService'VirtualUser':CaptureController()
      game:GetService'VirtualUser':Button1Down(Vector2.new(851, 158))
   end
   end)
   end)
   
   game:GetService("RunService").Heartbeat:Connect(function()
   pcall(function()
   if _G.AutoFarm or _G.NoClip or _G.elitehunt or _G.Electro or _G.AutoFarmBossHallow then
      game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
   end
   if _G.FastAttack or _G.AutoFarm then
      require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework.CameraShaker).CameraShakeInstance.CameraShakeState = {FadingIn = 3,FadingOut =  2,Sustained = 0,Inactive = 1}
   end
   if _G.bringmob and _G.AutoFarm then
      pcall(function()
      CheckQuest()
      for i,x in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
         for n,y in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
            if x.Name == Ms then
               if y.Name == Ms then
                  x.HumanoidRootPart.CFrame = y.HumanoidRootPart.CFrame
                  y.HumanoidRootPart.Size = Vector3.new(40,40,40)
                  x.HumanoidRootPart.Size = Vector3.new(40,40,40)
                  y.HumanoidRootPart.Transparency = 0.99
                  x.HumanoidRootPart.CanCollide = false
                  x.Humanoid.WalkSpeed = 0
                  x.Humanoid.JumpPower = 0
                  y.Humanoid.WalkSpeed = 0
                  y.Humanoid.JumpPower = 0
                  x.Humanoid:ChangeState(11)
                  y.Humanoid:ChangeState(11)
                  if sethiddenproperty then
                     sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
                  end
               end
            end
         end
      end
      end)
   end
   end)
   end)
   
   while wait(.1) do
      pcall(function()
      if _G.NoClip then
         game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
      end
      if _G.autoequipmelee then
         pcall(function()
         for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
            if v.ToolTip == "Melee" then
               if game.Players.LocalPlayer.Backpack:FindFirstChild(tostring(v.Name)) then
                  local ToolSe = tostring(v.Name)
                  local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
                  wait(.4)
                  game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
               end
            end
         end
         end)
      end
      if _G.autoequipsword then
         pcall(function()
         for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
            if v.ToolTip == "Sword" then
               if game.Players.LocalPlayer.Backpack:FindFirstChild(tostring(v.Name)) then
                  local ToolSe = tostring(v.Name)
                  local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
                  wait(.4)
                  game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
               end
            end
         end
         end)
      end
      if _G.Superhuman then
         pcall(function()
         if game.Players.LocalPlayer.Backpack:FindFirstChild("Combat") or game.Players.LocalPlayer.Character:FindFirstChild("Combat") then
            local args = {
               [1] = "BuyBlackLeg"
            }
            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
         end
         if game.Players.LocalPlayer.Character:FindFirstChild("Superhuman") or game.Players.LocalPlayer.Backpack:FindFirstChild("Superhuman") then
            _G.SelectWeapon = "Superhuman"
         end
         if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") or game.Players.LocalPlayer.Character:FindFirstChild("Electro") or game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") or game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") or game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") or game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") then
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value <= 299 then
               _G.SelectWeapon = "Black Leg"
            end
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value <= 299 then
               _G.SelectWeapon = "Electro"
            end
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value <= 299 then
               _G.SelectWeapon = "Fishman Karate"
            end
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value <= 299 then
               _G.SelectWeapon = "Dragon Claw"
            end
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value >= 300 then
               local args = {
                  [1] = "BuyElectro"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
            if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 300 then
               local args = {
                  [1] = "BuyElectro"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value >= 300 then
               local args = {
                  [1] = "BuyFishmanKarate"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
            if game.Players.LocalPlayer.Character:FindFirstChild("Electro") and game.Players.LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 300 then
               local args = {
                  [1] = "BuyFishmanKarate"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value >= 300 then
               local args = {
                  [1] = "BlackbeardReward",
                  [2] = "DragonClaw",
                  [3] = "1"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
               local args = {
                  [1] = "BlackbeardReward",
                  [2] = "DragonClaw",
                  [3] = "2"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
            if game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate").Level.Value >= 300 then
               local args = {
                  [1] = "BlackbeardReward",
                  [2] = "DragonClaw",
                  [3] = "1"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
               local args = {
                  [1] = "BlackbeardReward",
                  [2] = "DragonClaw",
                  [3] = "2"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value >= 300 then
               local args = {
                  [1] = "BuySuperhuman"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
            if game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw").Level.Value >= 300 then
               local args = {
                  [1] = "BuySuperhuman"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
         end
         end)
      end
      if _G.DeathStep then
         pcall(function()
         if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Backpack:FindFirstChild("Death Step") or game.Players.LocalPlayer.Character:FindFirstChild("Death Step") then
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value >= 450 then
               local args = {
                  [1] = "BuyDeathStep"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
               _G.SelectWeapon = "Death Step"
            end
            if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 450 then
               local args = {
                  [1] = "BuyDeathStep"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   
               _G.SelectWeapon = "Death Step"
            end
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value <= 449 then
               _G.SelectWeapon = "Black Leg"
            end
         else
            local args = {
               [1] = "BuyBlackLeg"
            }
            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
         end
         end)
      end
      if _G.Electro then
         pcall(function()
         if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") or game.Players.LocalPlayer.Character:FindFirstChild("Electro") or game.Players.LocalPlayer.Backpack:FindFirstChild("Electric Claw") or game.Players.LocalPlayer.Character:FindFirstChild("Electric Claw") then
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value >= 400 then
               local args = {
                  [1] = "BuyElectricClaw"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
               _G.SelectWeapon = "Electric Claw"
            end
            if game.Players.LocalPlayer.Character:FindFirstChild("Electro") and game.Players.LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 400 then
               local args = {
                  [1] = "BuyElectricClaw"
               }
               game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
   
               _G.SelectWeapon = "Electric Claw"
            end
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value <= 399 then
               _G.SelectWeapon = "Electro"
            end
         else
            local args = {
               [1] = "BuyElectro"
            }
            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
         end
         end)
      end
      if ThreeWorld then
         if _G.Electro then
            pcall(function()
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") or game.Players.LocalPlayer.Character:FindFirstChild("Electro") then
               if (game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value >= 400) or (game.Players.LocalPlayer.Character:FindFirstChild("Electro") and game.Players.LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 400) then
                  if _G.AutoFarm == false then
                     wait(1.1)
                     game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-10371.4717, 330.764496, -10131.4199, -0.804111481, 0, -0.594478488, 0, 1, 0, 0.594478488, 0, -0.804111481)
                     local args = {
                        [1] = "BuyElectricClaw",
                        [2] = "Start"
                     }
                     game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                     wait(2)
                     local Distancex = (Vector3.new(CFrame.new(-12550.532226563, 336.22631835938, -7510.4233398438)) - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
                     local Speexd = 100 -- ความเร็วของมึง
                     tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
                     tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(-12550.532226563, 336.22631835938, -7510.4233398438)})
                     tweenx:Play()
                     wait(Distancex/Speexd)
                     local Distancex = (Vector3.new(CFrame.new(-10371.4717, 330.764496, -10131.4199, -0.804111481, 0, -0.594478488, 0, 1, 0, 0.594478488, 0, -0.804111481)) - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
                     local Speexd = 100 -- ความเร็วของมึง
                     tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
                     tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(-10371.4717, 330.764496, -10131.4199, -0.804111481, 0, -0.594478488, 0, 1, 0, 0.594478488, 0, -0.804111481)})
                     tweenx:Play()
                     wait(Distancex/Speexd)
                     local args = {
                        [1] = "BuyElectricClaw"
                     }
                     game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                  elseif _G.AutoFarm == true then
                     _G.AutoFarm = false
                     game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-10371.4717, 330.764496, -10131.4199, -0.804111481, 0, -0.594478488, 0, 1, 0, 0.594478488, 0, -0.804111481)
                     local args = {
                        [1] = "BuyElectricClaw",
                        [2] = "Start"
                     }
                     game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                     wait(2)
                     game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-12550.532226563, 336.22631835938, -7510.4233398438)
                     wait(1)
                     game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-10371.4717, 330.764496, -10131.4199, -0.804111481, 0, -0.594478488, 0, 1, 0, 0.594478488, 0, -0.804111481)
                     local args = {
                        [1] = "BuyElectricClaw"
                     }
                     game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                     wait(.1)
                     _G.AutoFarm = true
                  end
               end
            end
            end)
         end
      end
   
      if  _G.elitehunt then
         if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
            local Distancex = (Vector3.new(CFrame.new(-5418.892578125, 313.74130249023, -2826.2260742188)) - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
            local Speexd = 100 -- ความเร็วของมึง
            tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
            tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = CFrame.new(-5418.892578125, 313.74130249023, -2826.2260742188)})
            tweenx:Play()
            wait(Distancex/Speexd)
            wait(.5)
            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EliteHunter")
         else
            if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text == "Defeat  Diablo (0/1)" then
               local magnitudez = (game:GetService("ReplicatedStorage")["Diablo [Lv. 1750]"].HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
               if magnitudez < 1000 then
                  if game:GetService("Workspace").Enemies:FindFirstChild("Diablo [Lv. 1750]") then
                     for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Diablo [Lv. 1750]" then
                           repeat wait()
                              itemequip(weapongg)
                              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,25,0)
                              v.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
                              v.HumanoidRootPart.CanCollide = false
                              v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                              v.Humanoid:ChangeState(11)
                              click()
                           until _G.elitehunt == false or v.Humanoid.Health <= 0
                        end
                     end
                  else
                     local Distancex = (game:GetService("ReplicatedStorage")["Diablo [Lv. 1750]"].HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
                     local Speexd = 150 -- ความเร็วของมึง
                     tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
                     tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("ReplicatedStorage")["Diablo [Lv. 1750]"].HumanoidRootPart.CFrame})
                     tweenx:Play()
                     wait(Distancex/Speexd)
                  end
               else
                  local Distancex = (game:GetService("ReplicatedStorage")["Diablo [Lv. 1750]"].HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
                  local Speexd = 150 -- ความเร็วของมึง
                  tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
                  tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("ReplicatedStorage")["Diablo [Lv. 1750]"].HumanoidRootPart.CFrame})
                  tweenx:Play()
                  wait(Distancex/Speexd)
               end
            elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text == "Defeat  Deandre (0/1)" then
               local magnitudez = (game:GetService("ReplicatedStorage")["Deandre [Lv. 1750]"].HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
               if magnitudez < 1000 then
                  if game:GetService("Workspace").Enemies:FindFirstChild("Deandre [Lv. 1750]") then
                     for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Deandre [Lv. 1750]" then
                           repeat wait()
                              itemequip(weapongg)
                              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,25,0)
                              v.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
                              v.HumanoidRootPart.CanCollide = false
                              v.Humanoid.WalkSpeed = 0
                              v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                              v.Humanoid:ChangeState(11)
                              click()
                           until _G.elitehunt == false or v.Humanoid.Health <= 0
                        end
                     end
                  else
                     local Distancex = (game:GetService("ReplicatedStorage")["Deandre [Lv. 1750]"].HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
                     local Speexd = 150 -- ความเร็วของมึง
                     tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
                     tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("ReplicatedStorage")["Deandre [Lv. 1750]"].HumanoidRootPart.CFrame})
                     tweenx:Play()
                     wait(Distancex/Speexd)
                  end
               else
                  local Distancex = (game:GetService("ReplicatedStorage")["Deandre [Lv. 1750]"].HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
                  local Speexd = 150 -- ความเร็วของมึง
                  tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
                  tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("ReplicatedStorage")["Deandre [Lv. 1750]"].HumanoidRootPart.CFrame})
                  tweenx:Play()
                  wait(Distancex/Speexd)
               end
            elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text == "Defeat  Urban (0/1)" then
               local magnitudez = (game:GetService("ReplicatedStorage")["Urban [Lv. 1750]"].HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
               if magnitudez < 1000 then
                  if game:GetService("Workspace").Enemies:FindFirstChild("Urban [Lv. 1750]") then
                     for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Urban [Lv. 1750]" then
                           repeat wait()
                              itemequip(weapongg)
                              game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0,25,0)
                              v.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame
                              v.HumanoidRootPart.CanCollide = false
                              v.Humanoid.WalkSpeed = 0
                              v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                              v.Humanoid:ChangeState(11)
                              click()
                           until _G.elitehunt == false or v.Humanoid.Health <= 0
                        end
                     end
                  else
                     local Distancex = (game:GetService("ReplicatedStorage")["Urban [Lv. 1750]"].HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
                     local Speexd = 150 -- ความเร็วของมึง
                     tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
                     tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("ReplicatedStorage")["Urban [Lv. 1750]"].HumanoidRootPart.CFrame})
                     tweenx:Play()
                     wait(Distancex/Speexd)
                  end
               else
                  local Distancex = (game:GetService("ReplicatedStorage")["Deandre [Lv. 1750]"].HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude -- จุดที่จะไป Position Only
                  local Speexd = 150 -- ความเร็วของมึง
                  tweenService, tweenInfo = game:GetService("TweenService"), TweenInfo.new(Distancex/Speexd, Enum.EasingStyle.Linear)
                  tweenx = tweenService:Create(game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart, tweenInfo, {CFrame = game:GetService("ReplicatedStorage")["Urban [Lv. 1750]"].HumanoidRootPart.CFrame})
                  tweenx:Play()
                  wait(Distancex/Speexd)
               end
            end
         end
      end
      if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
         local args = {
            [1] = "Buso"
         }
         game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
      end
      if _G.nododgecool then
         for i,v in next, getgc() do
            if game.Players.LocalPlayer.Character.Dodge then
               if typeof(v) == "function" and getfenv(v).script == game.Players.LocalPlayer.Character.Dodge then
                  for i2,v2 in next, getupvalues(v) do
                     if tostring(v2) == "0.4" then
                        repeat wait()
                           setupvalue(v,i2,0)
                        until not _G.nododgecool
                     end
                  end
               end
            end
         end
      end
      if InfinitsEnergy then
         wait(0.3)
         originalstam = LocalPlayer.Character.Energy.Value
         infinitestam()
      end
      if _G.BuySwordLegendary then
         local args = {
            [1] = "LegendarySwordDealer",
            [2] = "2"
         }
         game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
      end
      if _G.BuyHakiColorsDealer then
         game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ColorsDealer","2")
      end
      if _G.AutoFarmAllBoss then
         game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
      end
      if _G.AutoFarmMas then
         game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
      end
      if _G.AutoFarmMasGun then
         game:GetService("Players").LocalPlayer.Character.Humanoid:ChangeState(11)
      end
      end)
   end
   
   spawn(function()
      while wait(.1) do
            if Test == "Magnet" and AFM and StatrMagnet then
               CheckQuest()
               pcall(
                  function()
                        repeat
                           wait(.1)
                           for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                              if v.Name == Ms then
                                    wait()
                                    if HideHitBlox then
                                       v.HumanoidRootPart.Transparency = 1
                                    else
                                       v.HumanoidRootPart.Transparency = 0.75
                                    end
                                    v.HumanoidRootPart.CanCollide = false
                                    v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
                                    v.HumanoidRootPart.CFrame = PosMon
                              end
                           end
                        until LocalPlayer.PlayerGui.Main.Quest.Visible == false or AFM == false or StatrMagnet == false
                  end
               )
            end 
      end
   end)
   

