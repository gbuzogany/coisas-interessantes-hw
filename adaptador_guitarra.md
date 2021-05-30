

# Adaptador guitarra -> USB audio

### ADC (PCM1808)

Esse PCM1808 é um ADC com saída I2S. Podemos usar ele pra converter o sinal da guitarra pra um sinal digital que podemos manipular com microcontroladores ou uma FPGA.  
[Essa placa](https://www.aliexpress.com/item/32776593363.html?spm=a2g0s.9042311.0.0.27426c3790YhTa) é barata e já vem com os filtros analógicos que devemos precisar.

- [Datasheet](https://www.ti.com/lit/ds/sles177b/sles177b.pdf?ts=1622364785022)
- [Link Aliexpress](https://www.aliexpress.com/item/32776593363.html?spm=a2g0s.9042311.0.0.27426c3790YhTa)

### Microcontrolador (nrf52840)

O nrf52840 tem periféricos de I2S e um a interface PHY USB 2.0 integrada.  
O SDK da Nordic já tem código de exemplo pra usar o nrf52 como uma interface de audio USB, e outro exemplo de como usar a interface I2S.

- [Documentação exemplo USB Audio](https://infocenter.nordicsemi.com/topic/sdk_nrf5_v17.0.2/usbd_audio_example.html)
- [Documentação exemplo periférico I2S](https://infocenter.nordicsemi.com/topic/sdk_nrf5_v17.0.2/i2s_example_loopback.html)
- [Link download SDK](https://www.nordicsemi.com/Software-and-tools/Software/nRF5-SDK/Download)
- [Datasheet](https://infocenter.nordicsemi.com/pdf/nRF52840_PS_v1.1.pdf)
- [Link Aliexpress](https://www.aliexpress.com/item/1005001825655811.html?spm=a2g0o.productlist.0.0.447ee733LDUsk3&algo_pvid=e3768029-b486-49d5-bbf0-c891c7ffeb3a&algo_expid=e3768029-b486-49d5-bbf0-c891c7ffeb3a-3&btsid=0bb0623016223645238911192e0937&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_)
