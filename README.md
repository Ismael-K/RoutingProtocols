# RoutingProtocols



Implementation of the RIPv2, OSPF, BGP, EIGRP routing protocols from the Cisco Command Line on the Atlanta Router 192.168.2.2 in the network topology below.  This design can be simulated in Cisco Packet Tracer.

<p align="center">
  <img width="330" alt="topology" src="https://user-images.githubusercontent.com/17348315/40629255-ea536dac-6297-11e8-8c7a-48b16a51011d.PNG">

<p align="center">
<table class="tg">
  <tr>
    <th class="tg-yw4l"><b> </b></th>
    <th class="tg-yw4l"><b>RIPv2</b></th>
    <th class="tg-yw4l"><b>OSPF</b></th>
    <th class="tg-yw4l"><b>EIGRP</b></th>
    <th class="tg-yw4l"><b>BGP</b></th>
  </tr>
  <tr>
    <td class="tg-yw4l">Type:</td>
    <td class="tg-yw4l">Distance Vector</td>
    <td class="tg-yw4l">Link State</td>
    <td class="tg-yw4l">Distance Vector/hybrid</td>
    <td class="tg-yw4l">Path Vector</td>
  </tr>
  <tr>
    <td class="tg-yw4l">Algorithm:</td>
    <td class="tg-yw4l">Bellman Ford</td>
    <td class="tg-yw4l">Dijkstra</td>
    <td class="tg-yw4l">DUAL</td>
    <td class="tg-yw4l">Best Path Selection</td>
  </tr>
  <tr>
    <td class="tg-yw4l">Administrative Distance:</td>
    <td class="tg-yw4l">120</td>
    <td class="tg-yw4l">110</td>
    <td class="tg-yw4l">90</td>
    <td class="tg-yw4l">eBGP 20, iBGP 200</td>
  </tr>
  <tr>
    <td class="tg-yw4l">Metric:</td>
    <td class="tg-yw4l">Hop Count (Max = 15)</td>
    <td class="tg-yw4l">Cost</td>
    <td class="tg-yw4l">(BW + Delay)*256</td>
    <td class="tg-yw4l">MED</td>
  </tr> 
  <tr>
    <td class="tg-yw4l">Route Updates:</td>
    <td class="tg-yw4l">30 sec.</td>
    <td class="tg-yw4l">30 min. or topology change</td>
    <td class="tg-yw4l">Based on topology change</td>
    <td class="tg-yw4l">On topology change</td>
  </tr>
 <tr>
    <td class="tg-yw4l">Multicast Address:</td>
    <td class="tg-yw4l">224.0.0.9</td>
    <td class="tg-yw4l">224.0.0.5/224.0.0.6</td>
    <td class="tg-yw4l">224.0.0.10</td>
    <td class="tg-yw4l">-</td>
  </tr>
   <tr>
    <td class="tg-yw4l">Neighbor Adjacency Table:</td>
    <td class="tg-yw4l">N/A</td>
    <td class="tg-yw4l">Yes</td>
    <td class="tg-yw4l">Yes</td>
    <td class="tg-yw4l">Yes</td>
  </tr> 
    <tr>
    <td class="tg-yw4l">Transport Protocol:</td>
    <td class="tg-yw4l">UDP/520</td>
    <td class="tg-yw4l">IP/89</td>
    <td class="tg-yw4l">IP/88</td>
    <td class="tg-yw4l">TCP/179</td>
  </tr>
</table>




VLANsandVoip.pkt is a Packet Tracer file to simulate VoIP functionality on a network.  Router0 in the diagram below supports a trunk port to carry traffic for VLANs 1, 50, 99, 150.  Router0 is also configured as a DHCP server to provide network parameters to the VoIP phones.  

<p align="center">
<img width="451" alt="vlansandvoip" src="https://user-images.githubusercontent.com/17348315/41727595-b54f442e-7542-11e8-86b5-90c96a0acf31.PNG">
