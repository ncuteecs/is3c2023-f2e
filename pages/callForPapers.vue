<template>
  <Main pageName="Call For Papers">
    <ContentBlock title="Call For Papers">
      The International Symposium on Computer, Consumer and Control
      (<b>IS3C2020</b>) sponsored by National Chin-Yi University of Technology,
      held on November 13-16, 2020. This conference offers an excellent
      opportunity for scientists, engineers, and practitioners to present the
      latest research results, ideas, developments, and applications. IS3C, held
      every two years, is hosted by National Chin-Yi University of Technology,
      Taichung, Taiwan. As suggested by the name of the conference, the themes
      of this conference cover computer, multimedia and intelligent,
      communication application, integrated circuits, consumer electronics,
      renewable energy, systems and control, and digital signal processing.
      Original high-quality papers related to these themes are especially
      solicited, including theories, methodologies, and applications in
      Computing, Consumer, and Control. Selected papers will be published in the
      conference proceedings, and some excellent articles will be recommended to
      related SCI(E)/ EI journals for publication.
    </ContentBlock>

    <ContentBlock title="Invited Sessions" level="2">
      The IS3C2020 welcomes proposals for organizing special sessions within the
      conference scope. A brief statement of the session in one page must be
      submitted to
      <a class="link" href="mailto:is3c2020@ncut.edu.tw">is3c2020@ncut.edu.tw</a
      >. The organizer will be informed the acceptance soon after the proposal
      is approved.
      <br />
      <br />
      <center>
        <a class="link" href="http://is3c2020.ncuteecs.org/cfp.php#">
          Proceedings of IS3C2020 will be submitted to IEEE Xplore as well as EI
          index.</a
        >
      </center>
    </ContentBlock>
    <hr />
    <ContentBlock>
      Original papers describing current researches in the following themes are
      invited but not limited in.<br />
      <br />
      <TrackCard
        v-for="(track, i) in tracks"
        :key="track.name"
        v-bind="{ index: i, ...track }"
      />
    </ContentBlock>
  </Main>
</template>

<script>
export default {
  name: 'CallForPapers',
  data() {
    return {
      tracks: [
        {
          name: 'COMPUTER',
          descriptions: [
            'Computer Networks, Mobile Computing and Cloud Computing Technologies',
            'Digital Content and Web Service',
            'Software Engineering, Service-Oriented Architecture and Databases',
            'Artificial Intelligence, Knowledge Discovery and Fuzzy Systems',
            'Meta-Heuristic Algorithms and Optimization',
            'Information Security, Digital Right and Watermarking',
          ],
        },
        {
          name: 'MULTIMEDIA & INTELLIGENT COMPUTING',
          descriptions: [
            'Hardware and Software for Multimedia Systems',
            'Virtual Reality, AR, MR, 3D Processing and Application',
            'Signal, Audio, Speech Analysis and Processing',
            'Image Processing and Applications',
            'Computer Vision, Motion, Tracking Algorithms and Applications',
          ],
        },
        {
          name: 'COMMUNICATION APPLICATION',
          descriptions: [
            'Broadband Mobile and Wireless Communications',
            'Internet of Things (IoT) and Machine-to-Machine (M2M) Communication',
            'Sensor Networks, RFID Technology and Applications',
            'Big Data in Communications',
            'High Frequency and Microwave Circuits',
            'Radio and Microwave Engineering',
          ],
        },
        {
          name: 'INTEGRATED CIRCUITS',
          descriptions: [
            'Systems on Chip',
            'Application of Microelectronics ',
            'Device Modeling, Simulation and Design ',
            'Material and New Fabrication Facilities Technologies ',
            'Nano Technology ',
            'Sensors, Sensing Technology and Sensor Materials',
            'Micro Electro Mechanical Systems',
            'Microactuators',
          ],
        },
        {
          name: 'CONSUMER ELECTRONICS',
          descriptions: [
            'Human-Machine Interfaces',
            'Intelligent Robot and Its Applications',
            'Computer and Microprocessor-Based Control',
            'Home/Automotive Electronics Design',
            'Signal Processing in Measurement',
            'Sensor Applications',
            'Low Power Circuit Design',
          ],
        },
        {
          name: 'RENEWABLE ENERGY',
          descriptions: [
            'Renewable Energy Technologies',
            'Photovoltaic and Wind Energy Technologies',
            'Power Conversions of Renewable Energy',
            'Applications of Power Electronics in Power Systems',
            'Smart Grid Systems',
            'Applications of Renewable Energy in Wireless Charging Systems',
          ],
        },
        {
          name: 'SYSTEMS AND CONTROL',
          descriptions: [
            'System Modeling and Simulation, Dynamics and Control',
            'Intelligent and Learning Control ',
            'Robotics and Mechatronics',
            'Robust and Nonlinear Control',
            'Biomedical Systems and Control',
          ],
        },
        {
          name: 'DIGITAL SIGNAL PROCESSING',
          descriptions: [
            'Digital Signal Processing Theory and Methods',
            'Statistical Signal Processing and Applications',
            'Biomedical and Biological Signal Processing',
            'Neural Networks, Fuzzy Systems, Expert Systems, Genetic Algorithms and Data Fusion for Signal Processing',
            'Embedded Systems for Signal Processing',
          ],
        },
      ],
    }
  },
}
</script>
