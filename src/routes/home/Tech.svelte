<script>
  import flyte from '$lib/flyte.jpg';
  import telemetry from '$lib/telemetry.jpg';
</script>

<div id="tech">
  <h2>Feat. the <span id="hottest">Hottest</span> Tech</h2>
  <ul>
    <li>
      <h3>FLYTE</h3>

      <p>
        Our latest flight computer.

        <a href="https://github.com/IITB-Rocket-Team-Avionics/FLYTE"
          >Check it out on Github</a
        >
      </p>

      <img src={flyte} alt="FLYTE computers" />
      <span>2 years of PCB redesign.</span>
    </li>

    <li>
      <h3>Ground Station</h3>

      <p>
        Stream and view telemetry in realtime.

        <a href="https://github.com/jjbel/pi-pico-telemetry"
          >Check it out on Github</a
        >
      </p>

      <img src={telemetry} alt="" />
      <span>Data being streamed, denoised, and graphed in realtime</span>
    </li>

    <li>
      <h3>Payload Tracking</h3>

      <p>
        Advanced 4-axis gyro tracking and payload detection using Neural
        Networks.

        <!-- <a href="https://github.com/jjbel/pi-pico-telemetry"
          >Check it out on Github</a
          TODO
        > -->
      </p>

      <!-- <img src={telemetry} alt="" /> -->
      <!-- <span>Data being streamed, denoised, and graphed in realtime</span> -->
    </li>
  </ul>
</div>

<style>
  #tech {
    padding: 2vh 10% 2vh 10%;
  }

  h2 {
    font-size: 3.2rem;
    vertical-align: middle;
  }

  #hottest {
    font-family: 'Yellowtail', serif;
    font-size: 4.5rem;
    padding-right: 1.1rem;

    background: linear-gradient(to right, #ff2066, #ff5618);
    background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  ul {
    font-size: 1.4rem;
    margin-top: 0.2rem;

    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 1rem;
  }

  ul p {
    font-size: 1rem;
    margin-top: 1rem;
  }

  li {
    background-color: rgba(104, 104, 104, 0.13);
    padding: 0.8rem;
    border-radius: 0.6rem;
    width: 22rem;
    height: fit-content;
  }

  img {
    display: block;
    width: 100%;
    margin-top: 1rem;
  }

  ul span {
    color: rgb(220, 220, 220);
    font-size: 1rem;
  }

  ul a {
    text-decoration: underline;
  }
</style>
