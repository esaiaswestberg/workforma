<script lang="ts">
  import FormTable from '$components/dashboard/FormTable.svelte'
  import PageContainer from '$components/general/PageContainer.svelte'
  import PageTitle from '$components/general/PageTitle.svelte'
  import Header from '$components/navigation/Header.svelte'
</script>

<svelte:head>
  <title>App Dashboard - Workforma</title>
</svelte:head>

<Header />

<PageContainer>
  <PageTitle>Dashboard</PageTitle>
  <FormTable />
</PageContainer>
