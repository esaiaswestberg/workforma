<script lang="ts">
  const forms = [
    { name: 'Rental Agreement Form', protected: true, answers: 13 },
    { name: 'Employment Application', protected: false, answers: 34 },
    { name: 'Survey Feedback Form', protected: true, answers: 4 },
    { name: 'Event Registration Form', protected: false, answers: 149 },
    { name: 'Warranty Claim Form', protected: true, answers: 14 },
    { name: 'Volunteer Sign-Up Sheet', protected: false, answers: 7 },
    { name: 'Incident Report Form', protected: true, answers: 5 },
    { name: 'Scholarship Application', protected: true, answers: 44 },
    { name: 'Customer Feedback Survey', protected: false, answers: 180 },
    { name: 'Health Declaration Form', protected: false, answers: 21 }
  ]
</script>

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Protected</th>
      <th>Answers</th>
      <th>Actions</th>
    </tr>
  </thead>
  <tbody>
    {#each forms as form}
      <tr>
        <td>{form.name}</td>
        <td>{form.protected ? 'Private' : 'Public'}</td>
        <td>{form.answers}</td>
        <td>
          <button>Share</button>
          <button>Edit</button>
          <button>Delete</button>
        </td>
      </tr>
    {/each}
  </tbody>
</table>

<style>
  table {
    width: 100%;
  }

  th {
    font-weight: 600;
    text-align: left;
    padding: 0.5rem 0.25rem;
    border-bottom: 1px solid #ccc;
  }

  td {
    font-weight: 400;
    padding: 0.25rem;
  }

  tr:nth-child(even) {
    background-color: #f2f2f2;
  }

  th:last-child,
  td:last-child {
    display: flex;
    justify-content: end;
    gap: 0.5rem;
  }

  button {
    padding: 0.25rem 0.5rem;

    border: 1px solid #ccc;
    border-radius: 0.2rem;
    background-color: #fff;

    cursor: pointer;
  }

  button:hover {
    background-color: #eee;
    border-color: #aaa;
  }
</style>
