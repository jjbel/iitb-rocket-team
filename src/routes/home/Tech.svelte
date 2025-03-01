<script>
  import flyte from '$lib/flyte.jpg';
  import telemetry from '$lib/telemetry.jpg';
</script>

<div id="tech">
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
  ul {
    margin-top: 0.2rem;

    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 1rem;
  }

  ul p {
    font-size: 1.07rem;
    margin-top: 1rem;
  }

  li {
    background-color: rgba(155, 155, 155, 0.13);
    padding: 0.8rem;
    border-radius: 0.6rem;
    width: 22rem;
    height: fit-content;
  }

  :global(body.dark) li {
    background-color: rgba(104, 104, 104, 0.23);
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
