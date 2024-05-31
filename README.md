# 📝 API Documentation

## 📌 Table of Contents
1. [Account Information](https://github.com/jinix6/free-ff-api?tab=readme-ov-file#-account-information)
2. [Player Stats](https://github.com/jinix6/free-ff-api?tab=readme-ov-file#-player-stats)
3. [Craftland Profile Information](https://github.com/jinix6/free-ff-api?tab=readme-ov-file#%EF%B8%8F-craftland-profile-information)
4. [Craftland Map Information](https://github.com/jinix6/free-ff-api?tab=readme-ov-file#-craftland-map-information)
5. [WishList Items](https://github.com/jinix6/free-ff-api#wishlist-items)
6. [Error Responses](https://github.com/jinix6/free-ff-api#-error-responses)

# 🪪 Account Information
**Endpoint:** `/api/v1/account`  
**Method:** `GET`  
**Description**
This endpoint retrieves account information based on the specified region and user ID.

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`IND`, `BR`, `SG`, `RU`, `ID`, `TW`, `US`, `VN`, `TH`, `ME`, `PK`).|
| `uid`     | string | Yes      | The user ID.                  |
### 📨 Request Example
```http
GET https://free-ff-api.vercel.app/api/v1/account?region=IND&uid=1633864660
```


### 💬 Response Example
```json
{
  "basicInfo": {
    "accountId": "1633864660",
    "accountType": 1,
    "nickname": "╰ᴼᴰ╯✿Lɪᴘᴀɴ࿐",
    "region": "IND",
    "level": 73,
    "exp": 4027433,
    "bannerId": 901000009,
    "headPic": 902000045,
    "rank": 220,
    "rankingPoints": 3896,
    "badgeCnt": 105,
    "badgeId": 1001000072,
    "seasonId": 39,
    "liked": 20134,
    "showRank": true,
    "lastLoginAt": "1717066157",
    "csRank": 219,
    "csRankingPoints": 88,
    "weaponSkinShows": [
      907192607,
      912034002
    ],
    "maxRank": 220,
    "csMaxRank": 219,
    "accountPrefers": {},
    "createAt": "1574902662",
    "title": 904190039,
    "externalIconInfo": {
      "status": "ExternalIconStatus_NOT_IN_USE",
      "showType": "ExternalIconShowType_FRIEND"
    },
    "releaseVersion": "OB44",
    "showBrRank": true,
    "showCsRank": true,
    "socialHighLightsWithBasicInfo": {}
  },
  "profileInfo": {
    "avatarId": 102000007,
    "clothes": [
      50
    ],
    "equipedSkills": [
      211000032,
      205000059,
      214000067,
      203000191,
      204000515,
      211000859
    ],
    "pvePrimaryWeapon": 1,
    "endTime": 1,
    "clothesTailorEffects": [
      1
    ]
  },
  "historyEpInfo": [
    {
      "epEventId": 71,
      "epBadge": 1001000071,
      "badgeCnt": 128,
      "bpIcon": "UI_BP_Emoji_Pointed",
      "maxLevel": 100,
      "eventName": "T_43_H_BP71_NAME"
    },
    {
      "epEventId": 70,
      "ownedPass": true,
      "epBadge": 1001000070,
      "badgeCnt": 145,
      "bpIcon": "UI_BP_Emoji_Frog",
      "maxLevel": 100,
      "eventName": "T_43_H_BP70_NAME"
    },
    {
      "epEventId": 69,
      "epBadge": 1001000069,
      "badgeCnt": 151,
      "bpIcon": "UI_BP_Emoji_Asura",
      "maxLevel": 100,
      "eventName": "T_43_H_BP69_NAME"
    },
    {
      "epEventId": 68,
      "epBadge": 1001000068,
      "badgeCnt": 158,
      "bpIcon": "UI_BP_Emoji_Electri",
      "maxLevel": 150,
      "eventName": "T_42_H_BP68_NAME"
    },
    {
      "epEventId": 67,
      "epBadge": 1001000067,
      "badgeCnt": 139,
      "bpIcon": "UI_BP_Emoji_Watcher",
      "maxLevel": 150,
      "eventName": "T_42_H_BP67_NAME"
    },
    {
      "epEventId": 66,
      "epBadge": 1001000066,
      "badgeCnt": 128,
      "bpIcon": "UI_BP_Emoji_Puppets",
      "maxLevel": 150,
      "eventName": "T_42_H_BP66_NAME"
    },
    {
      "epEventId": 65,
      "epBadge": 1001000065,
      "badgeCnt": 150,
      "bpIcon": "UI_BP_Emoji_Fishing",
      "maxLevel": 150,
      "eventName": "T_41_JC_BP65_NAME"
    },
    {
      "epEventId": 64,
      "epBadge": 1001000064,
      "badgeCnt": 144,
      "bpIcon": "UI_BP_Emoji_Slime",
      "maxLevel": 150,
      "eventName": "T_41_JC_BP64_NAME"
    },
    {
      "epEventId": 63,
      "epBadge": 1001000063,
      "badgeCnt": 119,
      "bpIcon": "UI_BP_Emoji_Sonia",
      "maxLevel": 150,
      "eventName": "T_40_JC_BP63_NAME"
    },
    {
      "epEventId": 60,
      "epBadge": 1001000060,
      "badgeCnt": 127,
      "bpIcon": "UI_BP_Emoji_Rollerskating",
      "maxLevel": 150,
      "eventName": "T_39_FH_BP61_NAME"
    },
    {
      "epEventId": 59,
      "epBadge": 1001000059,
      "badgeCnt": 150,
      "bpIcon": "UI_BP_Emoji_Fishtank",
      "maxLevel": 150,
      "eventName": "T_39_FH_BP59_NAME"
    },
    {
      "epEventId": 58,
      "epBadge": 1001000058,
      "badgeCnt": 154,
      "bpIcon": "UI_BP_Emoji_Cybermech",
      "maxLevel": 150,
      "eventName": "T_38_FH_BP58_NAME"
    },
    {
      "epEventId": 57,
      "epBadge": 1001000057,
      "badgeCnt": 121,
      "bpIcon": "UI_BP_Emoji_Alligator",
      "maxLevel": 150,
      "eventName": "T_38_FH_BP57_NAME"
    },
    {
      "epEventId": 56,
      "epBadge": 1001000056,
      "badgeCnt": 127,
      "bpIcon": "UI_BP_Emoji",
      "maxLevel": 150,
      "eventName": "T_37_FH_BP56_NAME"
    },
    {
      "epEventId": 55,
      "ownedPass": true,
      "epBadge": 1001000055,
      "badgeCnt": 496,
      "eventName": "T_36_JL_EP55_BADGENAME"
    },
    {
      "epEventId": 54,
      "epBadge": 1001000054,
      "badgeCnt": 411,
      "eventName": "T_36_JL_EP54_BADGENAME"
    },
    {
      "epEventId": 53,
      "epBadge": 1001000053,
      "badgeCnt": 304,
      "eventName": "T_35_JL_EP53_BADGENAME"
    },
    {
      "epEventId": 52,
      "epBadge": 1001000052,
      "badgeCnt": 355,
      "eventName": "T_35_JL_EP52_BADGENAME"
    },
    {
      "epEventId": 51,
      "ownedPass": true,
      "epBadge": 1001000051,
      "badgeCnt": 460,
      "eventName": "T_34_JL_EP51_BADGENAME"
    },
    {
      "epEventId": 50,
      "epBadge": 1001000050,
      "badgeCnt": 263,
      "eventName": "T_34_JL_EP50_BADGENAME"
    }
  ],
  "clanBasicInfo": {
    "clanId": "3033195648",
    "clanName": "2ɢʙㅤᴏᴅɪsʜᴀ࿐",
    "captainId": "1633864660",
    "clanLevel": 3,
    "capacity": 30,
    "memberNum": 20
  },
  "captainBasicInfo": {
    "accountId": "1633864660",
    "accountType": 1,
    "nickname": "╰ᴼᴰ╯✿Lɪᴘᴀɴ࿐",
    "region": "IND",
    "level": 73,
    "exp": 4027433,
    "bannerId": 901000009,
    "headPic": 902000045,
    "rank": 220,
    "rankingPoints": 3896,
    "badgeCnt": 105,
    "badgeId": 1001000072,
    "seasonId": 39,
    "liked": 20134,
    "showRank": true,
    "lastLoginAt": "1717066157",
    "csRank": 219,
    "csRankingPoints": 88,
    "weaponSkinShows": [
      907192607,
      912034002
    ],
    "maxRank": 220,
    "csMaxRank": 219,
    "accountPrefers": {},
    "createAt": "1574902662",
    "title": 904190039,
    "externalIconInfo": {
      "status": "ExternalIconStatus_NOT_IN_USE",
      "showType": "ExternalIconShowType_FRIEND"
    },
    "releaseVersion": "OB44",
    "showBrRank": true,
    "showCsRank": true,
    "socialHighLightsWithBasicInfo": {}
  },
  "petInfo": {
    "id": 1300000001,
    "name": "Legend",
    "level": 6,
    "exp": 3018,
    "isSelected": true,
    "skinId": 1310000004,
    "selectedSkillId": 1315000010
  },
  "socialInfo": {
    "accountId": "1633864660",
    "gender": "Gender_MALE",
    "language": "Language_EN",
    "modePrefer": "ModePrefer_BR",
    "signature": "I may be slow to respond.",
    "rankShow": "RankShow_BR"
  },
  "diamondCostRes": {
    "diamondCost": 390
  },
  "creditScoreInfo": {
    "creditScore": 100,
    "rewardState": "REWARD_STATE_UNCLAIMED",
    "periodicSummaryLikeCnt": 30,
    "periodicSummaryIllegalCnt": 1,
    "periodicSummaryStartTime": "15",
    "periodicSummaryEndTime": "1716776753"
  },
  "equippedAch": [
    {
      "achId": 13002,
      "level": 3
    },
    {
      "achId": 13001,
      "level": 3
    },
    {
      "achId": 13006,
      "level": 3
    },
    {
      "achId": 13005,
      "level": 3
    }
  ]
}

```

# ⚙️ Craftland Profile Information
**Endpoint:** `/api/v1/craftlandProfile`  
**Method:** `GET`  
**Description:** Retrieve detailed information about a specific Craftland profile, including user statistics, created maps, resources used, and other related data.

### ☑️ Query Parameters
| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`IND`, `BR`, `SG`, `RU`, `ID`, `TW`, `US`, `VN`, `TH`, `ME`, `PK`).|
| `uid`     | string | Yes      | The user ID.                  |
### 📨 Request Example
```http
GET https://free-ff-api.vercel.app/api/v1/craftlandProfile?region=IND&uid=1633864660
```
### 💬 Response Example

```json

{
  "authorSlotsInfo": [
    {
      "slotId": 1,
      "slotState": "SlotState_PUBLISHED",
      "workshopCode": "2D1AA949DD77714ABB1FA0CE3ECCAFB34660",
      "workshopBasicInfo": {
        "workshopName": "FireZone",
        "authorId": "1633864660",
        "perfCost": "5",
        "updateTime": "1706154163",
        "resourceStatistics": "1",
        "authorName": "╰ᴼᴰ╯✿Lɪᴘᴀɴ࿐",
        "workshopDesc": "An exciting map in Craftland",
        "gameMode": 53,
        "tags": [
          17,
          25
        ],
        "modeSettings": "CoUHCgQIARgDCgIIGwoJCAgYAyUAAEBACgkIHRgFJQAAoEAKCggJGLQBJQAANEMKAggKCgkIBhgCJQAAAEAKCQgHGAElAACAPwoECAsQAQoJCAwYZCUAAMhCCgkIDRg8JQAAcEIKCQgcGDwlAABwQgoJCA4YFCUAAKBBCgIIAwoCCBoKAggFCgkIUhgCJQAAAEAKCggPGMgBJQAASEMKCggQGMgBJQAASEMKAggRCgIIEgoECBcQAQoDCJABCgMIkQEKAwiSAQoJCBMYZCUAAMhCCgkIFBhkJQAAyEIKCQgVGGQlAADIQgoJCBYYZCUAAMhCCgQIHhABCgQIHxABCgkIIBhkJQAAyEIKCQghGGQlAADIQgoJCCIYZCUAAMhCCgkIIxhkJQAAyEIKCQgkGGQlAADIQgoJCCUYZCUAAMhCCgkIJhhkJQAAyEIKAggnCgkIKBhkJQAAyEIKCQgpGGQlAADIQgoJCCoYZCUAAMhCCgkIKxhkJQAAyEIKCQgsGGQlAADIQgoKCEsY6AclAAB6RAoKCEwYyAElAABIQwoKCE0Y9AMlAAD6QwoECE4QAQoJCDEYPCUAAHBCCgkIMhhkJQAAyEIKCQgzGGQlAADIQgoJCDQYZCUAAMhCCgkINRhkJQAAyEIKCQg2GGQlAADIQgoJCDcYZCUAAMhCCgkIOBhkJQAAyEIKCQg5GGQlAADIQgoJCDoYZCUAAMhCCgkIPBhkJQAAyEIKCQg9GGQlAADIQgoJCD4YZCUAAMhCCgkIPxhkJQAAyEIKCQhAGGQlAADIQgoJCEEYZCUAAMhCCgkIQhhkJQAAyEIKCQhDGGQlAADIQgoJCEQYZCUAAMhCCgkIRRhkJQAAyEIKAghGCgkISBgPJQAAcEEKBAhJEAEKBAhKEAEKBAhYEAEKBAhZEAEKCQhaGB4lAADwQQoECFEQAQoJCF8YZCUAAMhCCgkIYBhkJQAAyEIKCQhhGGQlAADIQgoJCGIYZCUAAMhCCgoIngEYZCUAAMhCCgoIpgEYZCUAAMhCCgoIpwEYZCUAAMhCCgoIqAEYZCUAAMhCCgoIrwEYZCUAAMhCCgkIYxgBJQAAgD8KAghmCgkIZxgKJQAAIEEKAwiTAQoDCIEBCgUIggEQAQoFCI8BEAEKBQiNARABCgUIjgEQAQoDCJcBCgMImAEKAwiZAQoFCJoBEAEKAwibARgB",
        "teamCount": 2,
        "miniMapSettings": "AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA=",
        "miniMapObjectSettings": "CgcIjwEQFhgj",
        "mapId": 10,
        "commentInfo": {},
        "modeTemplateId": 3,
        "obVersion": 106,
        "createTime": "1706154163",
        "matchmakingRule": {}
      }
    }
  ],
  "accountInfo": {
    "exp": 20110,
    "createTimes": 5,
    "authorTag": 1
  },
  "authorId": "1633864660"
}
```

# 🏠 Craftland Map Information
**Endpoint:** `/api/v1/craftlandInfo`  
**Method:** `GET`  
**Description:** Retrieve detailed information about a specific Craftland map, including map details, resources used, and other related data.

### ☑️ Query Parameters

| Parameter  | Type   | Required | Description                                   |
|------------|--------|----------|-----------------------------------------------|
| `region`   | string | Yes      | The region code (`IND`, `BR`, `SG`, `RU`, `ID`, `TW`, `US`, `VN`, `TH`, `ME`, `PK`).                |
| `map_code` | string | Yes      | The unique code of the Craftland map.         |

### 📨 Request Example
```http
GET https://free-ff-api.vercel.app/api/v1/craftlandInfo?region=IND&map_code=2D1AA949DD77714ABB1FA0CE3ECCAFB34660
```

### 💬 Response Example

```json
{
  "workshopBasicInfo": {
    "workshopName": "FireZone",
    "authorId": "1633864660",
    "perfCost": "5",
    "updateTime": "1706154163",
    "resourceStatistics": "1",
    "authorName": "╰ᴼᴰ╯✿Lɪᴘᴀɴ࿐",
    "workshopDesc": "An exciting map in Craftland",
    "gameMode": 53,
    "tags": [
      17,
      25
    ],
    "modeSettings": "CoUHCgQIARgDCgIIGwoJCAgYAyUAAEBACgkIHRgFJQAAoEAKCggJGLQBJQAANEMKAggKCgkIBhgCJQAAAEAKCQgHGAElAACAPwoECAsQAQoJCAwYZCUAAMhCCgkIDRg8JQAAcEIKCQgcGDwlAABwQgoJCA4YFCUAAKBBCgIIAwoCCBoKAggFCgkIUhgCJQAAAEAKCggPGMgBJQAASEMKCggQGMgBJQAASEMKAggRCgIIEgoECBcQAQoDCJABCgMIkQEKAwiSAQoJCBMYZCUAAMhCCgkIFBhkJQAAyEIKCQgVGGQlAADIQgoJCBYYZCUAAMhCCgQIHhABCgQIHxABCgkIIBhkJQAAyEIKCQghGGQlAADIQgoJCCIYZCUAAMhCCgkIIxhkJQAAyEIKCQgkGGQlAADIQgoJCCUYZCUAAMhCCgkIJhhkJQAAyEIKAggnCgkIKBhkJQAAyEIKCQgpGGQlAADIQgoJCCoYZCUAAMhCCgkIKxhkJQAAyEIKCQgsGGQlAADIQgoKCEsY6AclAAB6RAoKCEwYyAElAABIQwoKCE0Y9AMlAAD6QwoECE4QAQoJCDEYPCUAAHBCCgkIMhhkJQAAyEIKCQgzGGQlAADIQgoJCDQYZCUAAMhCCgkINRhkJQAAyEIKCQg2GGQlAADIQgoJCDcYZCUAAMhCCgkIOBhkJQAAyEIKCQg5GGQlAADIQgoJCDoYZCUAAMhCCgkIPBhkJQAAyEIKCQg9GGQlAADIQgoJCD4YZCUAAMhCCgkIPxhkJQAAyEIKCQhAGGQlAADIQgoJCEEYZCUAAMhCCgkIQhhkJQAAyEIKCQhDGGQlAADIQgoJCEQYZCUAAMhCCgkIRRhkJQAAyEIKAghGCgkISBgPJQAAcEEKBAhJEAEKBAhKEAEKBAhYEAEKBAhZEAEKCQhaGB4lAADwQQoECFEQAQoJCF8YZCUAAMhCCgkIYBhkJQAAyEIKCQhhGGQlAADIQgoJCGIYZCUAAMhCCgoIngEYZCUAAMhCCgoIpgEYZCUAAMhCCgoIpwEYZCUAAMhCCgoIqAEYZCUAAMhCCgoIrwEYZCUAAMhCCgkIYxgBJQAAgD8KAghmCgkIZxgKJQAAIEEKAwiTAQoDCIEBCgUIggEQAQoFCI8BEAEKBQiNARABCgUIjgEQAQoDCJcBCgMImAEKAwiZAQoFCJoBEAEKAwibARgB",
    "teamCount": 2,
    "miniMapSettings": "AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA=",
    "miniMapObjectSettings": "CgcIjwEQFhgj",
    "mapId": 10,
    "commentInfo": {},
    "modeTemplateId": 3,
    "createTime": "1706154163",
    "matchmakingRule": {}
  }
}
```


# 📊 Player Stats

**Endpoint:** `/api/v1/playerstats`  
**Method:** `GET`  
**Description:** Retrieve detailed statistics for a specific player, including matches played, wins, kills, and other related data.

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                                   |
|-----------|--------|----------|-----------------------------------------------|
| `region`  | string | Yes      | The region code (`IND`, `BR`, `SG`, `RU`, `ID`, `TW`, `US`, `VN`, `TH`, `ME`, `PK`).                |
| `uid`     | string | Yes      | The user ID of the player.                    |

### 📨 Request Example
```http
GET https://free-ff-api.vercel.app/api/v1/playerstats?region=IND&uid=1633864660
```
### 💬 Response Example
```json
{
  "soloStats": {
    "accountId": "1633864660",
    "gamesPlayed": 12,
    "wins": 2,
    "kills": 55,
    "detailedStats": {
      "deaths": 10,
      "topNTimes": 5,
      "distanceTravelled": 45943,
      "survivalTime": 4585,
      "highestKills": 14,
      "damage": 17442,
      "headshots": 49,
      "headshotKills": 14,
      "pickUps": 1382
    }
  },
  "duoStats": {
    "accountId": "1633864660",
    "detailedStats": {}
  },
  "quadStats": {
    "accountId": "1633864660",
    "gamesPlayed": 26,
    "wins": 5,
    "kills": 110,
    "detailedStats": {
      "deaths": 21,
      "topNTimes": 9,
      "distanceTravelled": 112408,
      "survivalTime": 16246,
      "revives": 19,
      "highestKills": 11,
      "damage": 51276,
      "roadKills": 1,
      "headshots": 55,
      "headshotKills": 15,
      "knockDown": 123,
      "pickUps": 3133
    }
  }
}
```


# 🎫 Wishlist Items

**Endpoint:** `/api/v1/wishlistitems`  
**Method:** `GET`  
**Description:** Retrieve a list of items from a user's wishlist, including item IDs and their release times.

### ☑️ Query Parameters:

| Parameter | Type   | Required | Description                                   |
|-----------|--------|----------|-----------------------------------------------|
| `region`  | string | Yes      | The region code (`IND`, `BR`, `SG`, `RU`, `ID`, `TW`, `US`, `VN`, `TH`, `ME`, `PK`).                |
| `uid`     | string | Yes      | The user ID of the player.                    |

### 📨 Request Example
```http
GET https://free-ff-api.vercel.app/api/v1/wishlistitems?region=IND&uid=1187946149
```
### 💬 Response Example
```json
{
  "items": [
    {
      "itemId": 203043011,
      "releaseTime": "1707786123"
    },
    {
      "itemId": 204043011,
      "releaseTime": "1707786123"
    },
    {
      "itemId": 205043011,
      "releaseTime": "1707786123"
    },
    {
      "itemId": 211000589,
      "releaseTime": "1706471849"
    },
    {
      "itemId": 211043017,
      "releaseTime": "1707786123"
    },
    {
      "itemId": 904026008,
      "releaseTime": "1709657470"
    },
    {
      "itemId": 905042004,
      "releaseTime": "1715897897"
    }
  ]
}
```



# 😵 Error Responses
If there are errors in the request, the API will return an appropriate error message.

#### ⚠️ Error Example (Invalid uid)
```json
{
  "error": "Invalid request",
  "message": "Empty 'uid' parameter. Please provide a valid 'uid'."
}
```


#### ⚠️ Error Example (Invalid region)
```json
{
  "error": "Invalid request",
  "message": "Empty 'region' parameter. Please provide a valid 'region'."
}
```
```json
{
  "error": "Invalid request",
  "message": "Unsupported 'region' parameter. Supported regions are: IND, BR, SG, RU, ID, TW, US, VN, TH, ME, PK."
}
```


#### ⚠️ Error Example (Invalid map_code)
```json
{
  "error": "Invalid request",
  "message": "Empty 'map_code' parameter. Please provide a valid 'map_code'."
}
```





## ⭐️ Star Our Repository

If you find this project helpful, please consider giving it a star on GitHub! 🌟

Starring the repository helps us know that our work is valuable to you and motivates us to keep improving and adding new features.

[Star the Repository on GitHub](https://github.com/jinix6/free-ff-api)

Thank you for your support!
