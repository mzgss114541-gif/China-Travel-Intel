# Regional Hub Architecture (Strict 5-Hub Matrix)

All China travel intelligence dispatches, long-form guides, and regional advisories are categorized into the **5 Canonical Regional Hubs**.

---

## The 5 Regional Hubs

| Hub Code | Regional Focus & Key Destinations | English Post ID | Italian Post ID |
|:---|:---|:---:|:---:|
| `National_Policy_Transit` | Visa exemptions (15-day / 30-day), 144-Hour TWOV, customs regulations, CAAC aviation corridors, China Railway national trunk scheduling | **1227** | **1228** |
| `West_China` | Shaanxi (Xi'an), Sichuan (Chengdu, Jiuzhaigou), Yunnan (Lijiang, Shangri-La), Tibet (Lhasa), Xinjiang (Silk Road), Gansu (Dunhuang), Qinghai, Chongqing | **1243** | **1244** |
| `East_China` | Shanghai, Jiangsu (Suzhou, Nanjing), Zhejiang (Hangzhou, Ningbo), Anhui (Huangshan), Jiangxi (Jingdezhen, Wuyuan), Shandong, Fujian | **1252** | **1253** |
| `South_China` | Guangdong (Guangzhou, Shenzhen, GBA), Guangxi (Guilin, Yangshuo), Hainan (Sanya luxury coast), Hunan (Zhangjiajie, Fenghuang), Hubei (Three Gorges, Wuhan) | **1256** | **1257** |
| `North_China` | Beijing (Forbidden City, Great Wall), Tianjin, Hebei, Shanxi (Datong, Pingyao), Henan (Luoyang), Inner Mongolia, Jilin (Changbaishan), Heilongjiang (Harbin Ice Festival), Liaoning | **1258** | **1259** |

---

## Canonical Mapping Rules

### Central China Province Allocation
> [!IMPORTANT]
> **No Separate Central China Category**: Central China does NOT exist as an independent post or feed category in the system. Inland and central provinces are strictly mapped to adjacent hubs according to international traveler flow patterns:
> - **Hunan & Hubei** → `South_China` (grouped alongside Guangdong, Guangxi, Hainan)
> - **Jiangxi & Anhui** → `East_China` (grouped alongside Shanghai, Jiangsu, Zhejiang, Fujian, Shandong)
> - **Henan & Shanxi** → `North_China` (grouped alongside Beijing, Tianjin, Hebei, Inner Mongolia, Northeast)

---

## Hub Content Files in this Repository

- **National Policy & Transit**:
  - English: [`content/intelligence-hubs/en/national-policy-transit.md`](../content/intelligence-hubs/en/national-policy-transit.md)
  - Italian: [`content/intelligence-hubs/it/national-policy-transit.md`](../content/intelligence-hubs/it/national-policy-transit.md)
- **West China**:
  - English: [`content/intelligence-hubs/en/west-china.md`](../content/intelligence-hubs/en/west-china.md)
  - Italian: [`content/intelligence-hubs/it/west-china.md`](../content/intelligence-hubs/it/west-china.md)
- **East China**:
  - English: [`content/intelligence-hubs/en/east-china.md`](../content/intelligence-hubs/en/east-china.md)
  - Italian: [`content/intelligence-hubs/it/east-china.md`](../content/intelligence-hubs/it/east-china.md)
- **South China**:
  - English: [`content/intelligence-hubs/en/south-china.md`](../content/intelligence-hubs/en/south-china.md)
  - Italian: [`content/intelligence-hubs/it/south-china.md`](../content/intelligence-hubs/it/south-china.md)
- **North China**:
  - English: [`content/intelligence-hubs/en/north-china.md`](../content/intelligence-hubs/en/north-china.md)
  - Italian: [`content/intelligence-hubs/it/north-china.md`](../content/intelligence-hubs/it/north-china.md)
