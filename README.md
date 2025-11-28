
Hướng dẫn thiết lập môi trường cho PSoC E84

# Cần cài MobusToolbox v3.2
ModusToolbox là bộ công cụ phát triển chính thức của Infineon dành cho các dòng MCU như PSoC, PSoC Edge, XMC, Traveo…

Nó tích hợp sẵn GCC Arm toolchain, Eclipse IDE, BSP, HAL, PDL và nhiều công cụ sẵn khác

BSP (Board Support Package) gói phần mềm cung cấp mọi thứ cần thiết để ModusToolbox biết cách sử dụng board phần cứng cụ thể

PDL (Peripheral Driver Library)




# Cần cài EAP (Early Access Pack)
Gói mở rộng giúp ModusToolbox hỗ trợ các MCU mới phát hành, chẳng hạn như PSoC Edge E84

Pack này sẽ chứa BSP, PDL/HAL, ...




# Setup biến môi trường 
Cần thiết lập biến MTB_ENABLE_EARLY_ACCESS để Mobus có thể sử dụng pack early


# Python và edgeprotecttools
EdgeProtectTools là bộ công cụ phục vụ secure boot và ký firmware cho PSoC Edge E84

Nó được cài qua Python (pip) và bao gồm:

Công cụ ký image (image signing)

Các script để chuẩn bị firmware trước khi nạp

Hỗ trợ chuỗi secure boot của E84

EdgeProtectTools yêu cầu Python 3.8–3.12 


# Lưu ý khác
Để nạp code cho E84, nếu dùng KitProg3 hãy đảm bảo phiên bản firmware của nó là 2.60.1412


On the PSOC™ Edge E84 Evaluation kit (KIT_PSOCE84_EVK) please ensure below jumper and pin configuration
are correctly placed on board.


Ensure Boot.1(Boot SW) Pin(P17.6) should be in 'High'/ON position


Ensure J20 and J21 should be in Tristate/Not-Connected(NC) position
