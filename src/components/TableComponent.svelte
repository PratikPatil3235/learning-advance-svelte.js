<script>
  import { each } from "svelte/internal";

  const details = [
    {
      patientName: "Pratik",
      providerName: "Someone",
      service: "something",
      appointmentDate: "2016-06-17",
      appointmentTime: "07:30 am",
      status: true,
      scheduledOn: "2025-08-17",
      action: "",
    },
    {
      patientName: "Pratik",
      providerName: "Someone",
      service: "something",
      appointmentDate: "2016-06-17",
      appointmentTime: "07:30 am",
      status: true,
      scheduledOn: "2025-08-17",
      action: "",
    },
    {
      patientName: "Pratik",
      providerName: "Someone",
      service: "something",
      appointmentDate: "2016-06-17",
      appointmentTime: "07:30 am",
      status: true,
      scheduledOn: "2025-08-17",
      action: "",
    },
    {
      patientName: "Pratik",
      providerName: "Someone",
      service: "something",
      appointmentDate: "2016-06-17",
      appointmentTime: "07:30 am",
      status: true,
      scheduledOn: "2025-08-17",
      action: "",
    },
    {
      patientName: "Pratik",
      providerName: "Someone",
      service: "something",
      appointmentDate: "2016-06-17",
      appointmentTime: "07:30 am",
      status: true,
      scheduledOn: "2025-08-17",
      action: "",
    },
  ];
</script>

<main>
  <table>
    <thead>
      <tr>
        <th>Patient Name</th>
        <th>Provide Name</th>
        <th>Service</th>
        <th>Appt. Date</th>
        <th>Appt. Time</th>
        <th>Status</th>
        <th>Scheduled On</th>
        <th>Action</th>
      </tr>
    </thead>
    <tbody>
      {#each details as detail}
        <tr>
          <td>{detail.patientName}</td>
          <td>{detail.providerName}</td>
          <td>{detail.service}</td>
          <td>{detail.appointmentDate}</td>
          <td>{detail.appointmentTime}</td>
          <td>{detail.status}</td>
          <td>{detail.scheduledOn}</td>
          <td>{detail.action}</td>
        </tr>
      {/each}
    </tbody>
  </table>
</main>

<style>
  table {
    width: 70%;
    border-collapse: collapse;
    border: none;
    margin-top: 1rem;
    margin-left: 100px;
  }

  th, td {
    padding: 8px 12px; 
    text-align: left;
    border: 1px solid #ccc; 
  }

  thead {
    background-color: #f9f9f9;
  }

  tr:nth-child(even) {
    background-color: #f2f2f2; 
  }

  main{
    display: flex;
    align-items: center;
    justify-content:center;
    height: 100vh;
  }
</style>

