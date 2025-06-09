# 🛡️ GNS 보안 인프라 통합 구축 (GNS Security Infrastructure Integration Project)


![GNS 포폴](https://github.com/whathekim/GNSArchitecture/raw/main/GNS%20%ED%8F%AC%ED%8F%B4.PNG)
![GNS ASAv 정책](https://github.com/whathekim/GNSArchitecture/raw/main/GNS%20ASAv%20%EC%A0%95%EC%B1%85.PNG)


## 🔍 프로젝트 개요  
KOREAIT 아카데미 보안 과정 중 진행한 개인 실습으로, 기업 환경을 가정한 보안 인프라 모델링 및 구축에 중점을 두었습니다.  
내부망 보호와 외부 위협 대응을 위한 방화벽, IDS/IPS, SIEM, WAF 등의 구성 요소를 통합하고, VPN·모니터링·CTF 실습 환경까지 포함한 실제와 유사한 보안 아키텍처를 설계·구현하였습니다.

---

## 🧩 인프라 구성 개요

- **네트워크 분리 및 트래픽 제어**: ASA 방화벽, L2/L3 스위칭, VLAN 및 ACL 구성
- **침입 탐지 및 방어**: Snort, Suricata, iptables 기반 IDS/IPS 구성
- **웹 보안**: WAF 설정을 통한 OWASP Juice Shop 보호
- **로그 분석 및 위협 탐지**: Wazuh SIEM 및 OSSEC 연동
- **시스템 모니터링**: Zabbix와 PMM을 통한 성능 및 리소스 감시
- **보안 실습 환경 구성**: Kali Linux 기반 CTF 머신 구축 및 공격 테스트
- **VPN 구축**: pfSense를 활용한 외부 안전 접속 환경 구현

---

## ⚙️ 주요 구성 요소

| 구성 요소 | 역할 |
|-----------|------|
| **FW-ASA** | 내부/외부망 트래픽 제어 및 DMZ 분리 |
| **Router (ACL)** | 네트워크 접근 제어 |
| **Snort / Suricata** | 네트워크 기반 침입 탐지 및 차단 |
| **WAF** | 웹 애플리케이션 공격 방어 (OWASP Top10 대응) |
| **Wazuh + OSSEC** | 로그 수집 및 실시간 위협 탐지 (HIDS 포함) |
| **Loganalyzer** | 웹 기반 로그 분석 툴 |
| **Zabbix / PMM** | 시스템 상태 및 DB 성능 모니터링 |
| **pfSense VPN** | 외부 사용자 안전 접속 지원 |
| **CTF 머신 / Juice Shop** | 모의해킹 실습 환경 제공 |
| **Internal PC & DNS/DB Server** | 사용자 환경 및 네트워크 서비스 구성 |

---

## 🛠️ 사용 기술 스택

- **네트워크**: VLAN, Routing, DMZ, ACL, L2/L3 Switching  
- **보안 장비**: Cisco ASA, pfSense, iptables  
- **침입 탐지/방어**: Snort, Suricata, WAF  
- **로그/시스템 분석**: Wazuh, OSSEC, Loganalyzer  
- **모니터링**: Zabbix, PMM  
- **보안 실습 환경**: OWASP Juice Shop, CTF Machine, Kali Linux  
- **운영체제**: Rocky Linux 8.10, Ubuntu 24.04

---

## 🎯 프로젝트 목표 및 결과

- 내부망과 DMZ를 분리하여 보안 경계를 명확히 구축  
- IDS/IPS 및 WAF 구성으로 다계층 보안 체계 수립  
- Wazuh SIEM 도입으로 로그 기반 위협 분석 체계화  
- Kali를 활용한 공격 시나리오 수행 및 취약점 보고서 작성  
- Zabbix/PMM을 활용한 실시간 리소스 모니터링 구현  

---

## 👤 개인 담당 역할

- 전체 보안 인프라 설계 및 GNS3 시뮬레이션 구축  
- ASA 방화벽 및 pfSense VPN 구성  
- Snort, Suricata, iptables 조합 IDS/IPS 설정  
- Wazuh + OSSEC 연동 및 SIEM 대시보드 구성  
- Kali Linux 기반 모의해킹 수행 및 결과 보고서 작성  

---

## 🔭 향후 발전 방향

- ELK Stack 기반 통합 로그 분석 환경 구축  
- AWS, Azure 연동을 통한 클라우드 보안 실험  
- SOAR 기반 자동화 보안 대응 시나리오 연계  
