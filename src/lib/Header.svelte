<script>
    import SelfCard from "./SelfCard.svelte";
    import CollapsedMenu from "./CollapsedMenu.svelte";
    import TopicLink from "./TopicLink.svelte";
    import ContentModal from "./ContentModal.svelte";
</script>
<div class="h-18 w-full bg-blue-950 flex flex-row justify-between items-center sticky top-0 flex-nowrap space-x-4 p-4" >
    <SelfCard></SelfCard>
    <ContentModal heading="Menú" >
        <CollapsedMenu heading={"Secciones"} >
            <TopicLink link="./sections/section1" >
                Sección #1
            </TopicLink>
            <TopicLink link="./sections/section2" >
                Sección #2
            </TopicLink>
            <TopicLink link="./sections/section3" >
                Sección #3
            </TopicLink>
        </CollapsedMenu>
    </ContentModal>
</div>