<template>
  <v-app>
    <v-main>
      <Header />
      <Animation />

      <v-container class="mt-10">
        <v-row>
          <v-col cols="12" sm="6" class="mr-auto">
            <base-heading
              class="text-left"
              :size="'text-h4'"
              title="The Scalable, Multichain Network for Radical Innovation"
            />
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12" sm="8" class="ml-auto">
            <base-heading
              class="text-left"
              :size="'text-h6'"
              title="Unprecedented interoperability and scalability for blockchain developers who want to quickly push the limits of what’s possible. Built using Substrate with nearly the same codebase and industry-leading multichain infrastructure as Kusama’s cousin, Polkadot."
            />
          </v-col>
        </v-row>

        <v-row class="mb-12">
          <v-col cols="12" class="text-center">
            <v-img
              src="@/assets/boxes_graph.png"
              class="shrink mr-2"
              contain
              width="100%"
            />
          </v-col>
        </v-row>
        <v-row class="mt-12">
          <v-col cols="12" sm="8" class="mr-auto">
            <base-heading
              class="text-left"
              :size="'text-h4'"
              title="Origin of Kusama"
            />
          </v-col>
        </v-row>

        <v-row>
          <v-col cols="12" sm="8" class="mr-auto">
            <base-heading
              class="text-left"
              :size="'text-h6'"
              title="The relationship between society and technology has deteriorated to the point where large entities routinely stretch and overstep their authority."
            />
          </v-col>
          <v-col cols="12" sm="8" class="mr-auto">
            <base-heading
              class="text-left"
              :size="'text-h6'"
              title="Kusama is a network built as a risk-taking, fast-moving ‘canary in the coal mine’ for its cousin Polkadot. It's a living platform built for change agents to take back control, spark innovation and disrupt the status quo."
            />
          </v-col>
        </v-row>

        <v-row class="paralax">
          <div class="col-md-6 ml-auto box-outlines" style="--progress:44%">
            <div class="col-md-12 mr-1 mt-1 ">
              <v-col cols="12" class="ml-auto">
                <base-heading
                  class="text-left"
                  :size="'text-h4'"
                  title="What is Kusama?"
                />
              </v-col>
              <v-col cols="12" class="ml-auto">
                <base-heading
                  class="text-left"
                  :size="'text-h6'"
                  title="Kusama is a scalable network of specialized blockchains built using Substrate and nearly the same codebase as Polkadot. The network is an experimental development environment for teams who want to move fast and innovate on Kusama, or prepare for deployment on Polkadot."
                />
              </v-col>
              <v-col cols="12" class="ml-auto">
                <base-heading
                  class="text-left"
                  :size="'text-h6'"
                  title="Kusama was founded in 2019 by Gavin Wood, founder of Polkadot and co-founder and former CTO of Ethereum."
                />
              </v-col>
            </div>
          </div>
        </v-row>
        <v-row class="mt-6">
          <v-col class="container" cols="12">
            <img src="@/assets/mesh_graph_1.png" />
            <div class="col-sm-6 display-2 text-left top-left">
              Launch your custom blockchain
            </div>
            <div class="col-sm-6 scroll_hide_bar top-right mt-6">
              <v-row v-for="item in dados1" :key="item.id">
                <v-list-item class="grow">
                  <v-list-item-avatar color="">
                    <v-img class="elevation-6" alt="" :src="item.icon"></v-img>
                  </v-list-item-avatar>

                  <v-list-item-content class="ml-0 text-left white--text">
                    <v-list-item-title class="display-1">{{
                      item.text
                    }}</v-list-item-title>
                  </v-list-item-content>
                </v-list-item>

                <!-- <v-col cols="12">
                  <v-card-title>
                    <v-icon large left color="white">
                      mdi-twitter
                    </v-icon>
                    <span class="display-1 text-left">{{ item.text }}</span>
                  </v-card-title>
                </v-col> -->
                <base-heading
                  class="text-left"
                  :size="'subtitle-1'"
                  :title="item.subtext"
                />
              </v-row>
            </div>
          </v-col>
        </v-row>
        <v-row class="mt-12">
          <v-col class="text-center">
            <v-btn color="red" outlined>
              Ready to Start? Contact our Team</v-btn
            >
          </v-col>
        </v-row>

        <v-row class="mt-12">
          <v-col cols="12" md="6" class="display-2 text-left">
            Bring to your project
          </v-col>
          <v-col cols="12" md="6" class="scroll_hide_bar  mt-6">
            <v-row v-for="item in dados2" :key="item.id">
              <v-list-item class="grow mx-0 px-0">
                <v-list-item-content class="mx-0 text-left white--text">
                  <v-list-item-title class="px-0 display-1">{{
                    item.text
                  }}</v-list-item-title>
                </v-list-item-content>
              </v-list-item>

              <base-heading
                class="text-left"
                :size="'subtitle-1'"
                :title="item.subtext"
              />
            </v-row>
          </v-col>
        </v-row>

        <v-row class="my-6">
          <v-col class="container" cols="12">
            <img src="@/assets/mesh_graph_2.png" />
            <div class="col-md-6 display-2  top-left text-left">
              Develop on the Canary Network
            </div>
            <!-- <div class="col-md-6"> -->
            <v-row>
              <v-col
                cols="12"
                md="6"
                class="subtitle-1 text-left bottom-right white--text"
              >
                Many teams will choose Kusama for their dapp or parachain and
                remain exclusively on Kusama. Other teams will join Kusama as a
                temporary preparation ground for deployment on Polkadot
              </v-col>
            </v-row>
            <!-- </div> -->
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12">
            <base-heading
              class="text-center"
              :size="'display-1'"
              :title="'Join the Kusama Ecosystem'"
            />
          </v-col>
        </v-row>
        <v-row>
          <v-col
            v-for="card in cards"
            :key="card.title"
            cols="12"
            sm="3"
            md="2"
          >
            <v-icon color="white" large>
              {{ card.icon }}
            </v-icon>
            <div>{{ card.title }}</div>
          </v-col>
        </v-row>
        <v-row class="mt-12">
          <v-col cols="12" md="6" class="display-2 text-left">
            Parachains and Applications
          </v-col>
          <v-col cols="12" md="4" offset-md="1" class="mt-6">
            <v-row v-for="item in dados3" :key="item.id">
              <v-list-item class="grow mx-0 px-0">
                <v-list-item-content class="mx-0 text-left white--text">
                  <v-list-item-title class="px-0 headline">{{
                    item.text
                  }}</v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-row>
          </v-col>
        </v-row>
        <v-row class="mt-12">
          <v-col class="text-center">
            <v-btn color="red" outlined> Why Build a Parachain</v-btn>
          </v-col>
        </v-row>

        <v-row class="mt-12">
          <v-col cols="12" md="6" class="display-2 text-left">
            KSM Token Utilization
          </v-col>
          <v-col cols="12" md="4" offset-md="1" class="mt-6">
            <v-row v-for="item in dados4" :key="item.id">
              <v-list-item class="grow mx-0 px-0">
                <v-list-item-content class="mx-0 text-left white--text">
                  <v-list-item-title class="px-0 headline text-wrap"
                    ><span class="font-weight-bold">{{ item.caps }}</span
                    >{{ item.text }}</v-list-item-title
                  >
                </v-list-item-content>
              </v-list-item>
            </v-row>
          </v-col>
        </v-row>

        <v-row class="my-12">
          <v-col cols="12" md="4" class="display-2 text-left">
            Built with Substrate
          </v-col>
          <v-col cols="12" md="6" offset-md="1" class="mt-6">
            <img
              src="@/assets/substrate-playground.png"
              alt="Substrate Playground"
              width="100%"
              class="mb-4"
            />
            <v-row no-gutters>
              <v-col cols="12">
                <base-heading
                  class="text-left mb-0"
                  :size="'subtitle-1'"
                  :title="
                    `Your Substrate Blockchain is natively compatible with Kusama, making it simple to secure your blockchain and communicate with Kusama's network.`
                  "
                />
              </v-col>
              <v-row class="mt-2">
                <v-col class="text-center">
                  <v-btn color="white" outlined class="mr-2">Learn More</v-btn>
                  <v-btn color="red" outlined>Substract Playground</v-btn>
                </v-col>
              </v-row>
            </v-row>
          </v-col>
        </v-row>

        <base-heading
          class="text-center"
          :size="'display-1 mt-12'"
          :title="`Take Flight`"
        />

        <v-row class="mt-6 justify-center">
          <v-col cols="12" md="4" sm="6" v-for="item in dados5" :key="item.id">
            <v-card
              color="black"
              class="box-outlines fill-height"
              style="--progress:44%"
            >
              <v-card-title class="display-1 white--text justify-center">
                <!-- <v-icon color="teal" class="a_link" v-if="confirm_modal_dialog_icon" left="true">{{ confirm_modal_dialog_icon }}</v-icon> -->
                {{ item.title }}
              </v-card-title>
              <v-card-text>
                <v-list color="black">
                  <v-list-item v-for="dta in item.listData" :key="dta.title">
                    <v-list-item-content>
                      <v-list-item-title
                        class="text-left white--text"
                        v-text="dta.title"
                      ></v-list-item-title>
                    </v-list-item-content>
                    <v-list-item-icon>
                      <v-icon v-if="dta.icon" color="pink">
                        {{ dta.icon }}
                      </v-icon>
                    </v-list-item-icon>
                  </v-list-item>
                </v-list>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
        <base-heading
          class="text-center"
          :size="'display-1 mt-12'"
          :title="`Stay in the Loop`"
        />
        <v-row class="justify-center">
          <v-col cols="4">
            <base-heading
              class="text-center"
              :size="'subtitle-2 mt-12'"
              :title="
                `Subscribe to the newsletter to hear about Kusama updates and events.`
              "
            />
            <div class="text-center">
              <v-btn color="red" outlined> Subscribe</v-btn>
            </div>
            <base-heading
              class="text-center"
              :size="'caption mt-6'"
              :title="
                `To see how we use your information please see our privacy policy.`
              "
            />
          </v-col>
        </v-row>

        <v-row class="mt-6">
          <v-col v-for="item in dados6" :key="item.id">
            <v-card color="black">
              <v-card-title class="headline white--text justify-left ml-4 pb-0">
                <!-- <v-icon color="teal" class="a_link" v-if="confirm_modal_dialog_icon" left="true">{{ confirm_modal_dialog_icon }}</v-icon> -->
                {{ item.title }}
              </v-card-title>
              <v-card-text>
                <v-list color="black">
                  <v-list-item v-for="dta in item.listData" :key="dta.title">
                    <v-list-item-content>
                      <v-list-item-title
                        class="text-left grey--text darken-1"
                        v-text="dta.title"
                      ></v-list-item-title>
                    </v-list-item-content>
                  </v-list-item>
                </v-list>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
        <base-heading
          class="text-center"
          :size="'caption mt-6'"
          :title="
            `© 2021 Kusama · Privacy Policy · Terms and Conditions · Cookie Settings`
          "
        />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import Header from "./components/Header";
import Animation from "./components/Animation";
import BaseHeading from "@/components/Heading";

export default {
  name: "App",

  components: {
    Header,
    Animation,
    BaseHeading,
  },

  data: () => ({
    cards: [
      {
        icon: "mdi-keyboard-outline",
        title: "Polkadot",
      },
      {
        icon: "mdi-keyboard-outline",
        title: "Acala",
      },
      {
        icon: "mdi-keyboard-outline",
        title: "Chainlink",
      },

      {
        icon: "mdi-keyboard-outline",
        title: "Moonbeam",
      },

      {
        icon: "mdi-keyboard-outline",
        title: "Phala",
      },

      {
        icon: "mdi-keyboard-outline",
        title: "Edgeware",
      },
    ],
    dados1: [
      {
        id: 1,
        icon:
          "data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E",
        text: "Fast Iteration",
        subtext:
          "Move fast and ship your product. Kusama’s risk-taking and nimble mentality allows developers to move swiftly through the governance and upgrade process, enabling rapid progress and growth.",
      },

      {
        id: 2,
        icon:
          "data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E",
        text: "Low Economic Barriers",
        subtext:
          "Launch your custom blockchain (parachain) project with low barriers to entry. Ideal for lean startups looking to move fast and iterate.",
      },

      {
        id: 3,
        icon:
          "data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E",
        text: "Advanced Technology",
        subtext:
          "Build on a next-generation, sharded, multichain network, while employing the newest features before they are deployed on Polkadot.",
      },

      {
        id: 4,
        icon:
          "data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E",
        text: "Open Governance",
        subtext:
          "Kusama is owned and governed by a community of network participants who vote on and control the evolution of the network. Have a voice and make your mark in the evolution of the network.",
      },

      {
        id: 5,
        icon:
          "data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E",
        text: "Engaged Community",
        subtext:
          "Leverage Polkadot’s global brand and developer community for your parachain, parathread or dApp.",
      },
      {
        id: 6,
        icon:
          "data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E",
        text: "Valuable Experience",
        subtext:
          "For teams looking to move to Polkadot after fine-tuning on Kusama, begin building your community and brand on Kusama before deployment.",
      },
    ],
    dados2: [
      {
        id: 1,
        text: "Innovation",
        subtext:
          "Kusama is built by the same teams as Polkadot, using nearly the same code and tools. The network places the latest tech from Parity Technologies and Web3 Foundation in the hands of developers, even before those features make it to Polkadot.",
      },
      {
        id: 2,
        text: "Scalability",
        subtext:
          "Kusama’s sharded blockchains and open governance provide a scalable and future-proof infrastructure for businesses, marketplaces and applications to deploy and mature.",
      },
      {
        id: 3,
        text: "Interoperability",
        subtext:
          "Kusama brings multiple blockchains together into one sharded network, freeing developers from the siloes created by legacy blockchain networks.",
      },

      {
        id: 4,
        text: "Customization",
        subtext:
          "With Substrate, developers can build their own app-specific blockchain and connect it to Kusama.",
      },
    ],
    dados3: [
      {
        id: 1,
        text: "Gaming and eSports",
      },
      {
        id: 2,
        text: "Messaging",
      },
      {
        id: 3,
        text: "DAO",
      },
      {
        id: 4,
        text: "Marketplaces",
      },
      {
        id: 5,
        text: "Oracles",
      },
      {
        id: 6,
        text: "Music",
      },
      {
        id: 7,
        text: "Social Networking",
      },
    ],

    dados4: [
      {
        id: 1,
        caps: "Validate ",
        text: "the network",
      },
      {
        id: 2,
        caps: "Nominate ",
        text: "validators",
      },
      {
        id: 3,
        caps: "Bond ",
        text: "parachains or parathreads",
      },

      {
        id: 4,
        caps: "Vote ",
        text: "on governance referenda",
      },
    ],

    dados5: [
      {
        id: 1,
        title: "Build",
        listData: [
          { id: 1, title: "Kusama Docs", icon: "mdi-arrow-right" },
          { id: 2, title: "Learn Substrate", icon: "mdi-arrow-right" },
        ],
      },
      {
        id: 2,
        title: "Validate",
        icon: "",
        listData: [
          { id: 1, title: "Start Validating", icon: "mdi-arrow-right" },
          { id: 2, title: "Technical Updates", icon: "mdi-arrow-right" },
        ],
      },
      {
        id: 3,
        title: "Join",
        icon: "",
        listData: [
          { id: 1, title: "Ambassador Program", icon: "mdi-arrow-right" },
          { id: 2, title: "Nominate a Validator", icon: "mdi-arrow-right" },
        ],
      },
    ],
    dados6: [
      {
        id: 1,
        title: "Developers",
        listData: [
          { id: 1, title: "Guide" },
          { id: 2, title: "GitHub" },
          { id: 3, title: "Technical Riot Chat" },
          { id: 4, title: "Web3 Foundation Grants" },
          { id: 5, title: "Governance Chat" },
          { id: 6, title: "Validator Chat" },
        ],
      },
      {
        id: 2,
        title: "Community",
        listData: [
          { id: 1, title: "Community Hub" },
          { id: 2, title: "Ambassador Program" },
          { id: 3, title: "Meetup Hub" },
          { id: 4, title: "Find a Local Meetup" },
          { id: 5, title: "Blog" },
          { id: 6, title: "Brand Assets" },
        ],
      },
      {
        id: 3,
        title: "Social",
        listData: [
          { id: 1, title: "Discord" },
          { id: 2, title: "Watercooler Riot Chat" },
          { id: 3, title: "Twitter" },
          { id: 4, title: "Reddit" },
          { id: 5, title: "YouTube" },
          { id: 6, title: "Crowdcast Webinars" },
        ],
      },
      {
        id: 4,
        title: "Info",
        listData: [
          { id: 1, title: "Support" },
          { id: 2, title: "Polkadot" },
          { id: 3, title: "Substrate" },
          { id: 4, title: "Careers" },
          { id: 5, title: "Web3 Foundation" },
          { id: 6, title: "Parity Technologies" },
        ],
      },
    ],
  }),
};
</script>
<style>
#app {
  background-color: black;
  color: white;
}

.box-outlines {
  display: inline-block;
  width: auto;
  position: relative;
  padding: 4rem 3rem !important;
}
.box-outlines::before,
.box-outlines::after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  border: solid 2px red;
  pointer-events: none;
}
.parallax .box-outlines::after {
  transform: translate3d(
    calc(var(--progress) / 20),
    calc(var(--progress) / 20),
    0
  );
}
.box-outlines::before {
  transform: translate3d(
    calc(var(--progress) / 20 * -1),
    calc(var(--progress) / 20 * -1),
    0
  );
}

.section-hero {
  max-width: 560px;
  position: relative;
  top: 0;
  left: -50px;
  transform: translateY(-100%);
  padding-right: 3rem;
}
.section-hero .bg-img img {
  max-width: 80%;
}
.section-hero .bg-img {
  opacity: 0.5;
  text-align: center;
}

.scroll_hide_bar {
  /* width: 200px; */
  height: 500px;
  /* border: 1px dotted black; */
  overflow-y: scroll; /* Add the ability to scroll */
}

/* Hide scrollbar for Chrome, Safari and Opera */
.scroll_hide_bar::-webkit-scrollbar {
  display: none;
}

/* Hide scrollbar for IE, Edge and Firefox */
.scroll_hide_bar {
  -ms-overflow-style: none; /* IE and Edge */
  scrollbar-width: none; /* Firefox */
}

.bg-img {
  position: absolute;
  margin: 0 auto;
  margin-top: 30px;
}
.bg-img img {
  max-width: 80%;
  /* transform: translateY(-30%); */
  /* transform: translateX(-15%); */
}

/* Container holding the image and the text */
.container {
  position: relative;
  text-align: center;
  color: white;
}

/* Bottom left text */
.bottom-left {
  position: absolute;
  bottom: 8px;
  left: 16px;
}

/* Top left text */
.top-left {
  position: absolute;
  top: 10%;
  left: 20px;
  display: inline-block;
}

/* Top right text */
.top-right {
  position: absolute;
  top: 8px;
  right: 16px;
}

/* Bottom right text */
.bottom-right {
  position: absolute;
  bottom: 10px;
  right: 16px;
}

/* Centered text */
.centered {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.icon_fast {
  -webkit-mask-image: url(data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E);
  mask-image: url(data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E);
}

/* .v-list-item__title {
  white-space: normal;
} */
</style>
